# préparation de disque :
-lsblk : **voir les répartitions** 
-fdisk /dev/sdb : **faire répartition sur le disque sdb**

*n* : **nouvelle partition**
*p* : **primaire +6G**
*n*
*p*
*t* : 82 : **swap**
mkfs.ext4 /dev/sdb1 : **formatage de partition sdb1 en ext4**
mkswap /dev/sdb2 : **Formatage la partition comme swap**
swapon /dev/sdb2 : **active le swap**
# montage :
mkdir -p mnt/DATA
blkid : **connaitre l'UUID de sdb1 "ext4"**
nano /etc/fstab ----> UUID /mnt/DATA défaults 0 0
mount -a : **teste le montage sans redémarrer**
df -h : **vérification si la partition sdb1 a bien montée à /mnt/DATA**                              
