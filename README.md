1.��ȡ���룬����

cd BootImgTool
chmod 755 build.sh
./build.sh


2.ʹ��tmp�µ�boot.img���֣������
./bin/unpack-bootimg.sh .tmp/boot.img

��ʱtmp���£�
ll tmp
total 34944
-rw-r--r--   1 andr0day  staff   8.5M  4 16 19:14 boot.img
-rw-r--r--   1 andr0day  staff   8.0M  4 16 19:30 boot.img-kernel.gz //�滻kernelʱ�����Ǵ��ļ�
drwxr-xr-x  25 andr0day  staff   800B  4 16 19:30 boot.img-ramdisk //�����Ŀ¼�޸�����
-rw-r--r--   1 andr0day  staff   488K  4 16 19:30 boot.img-ramdisk.cpio.gz


3.�޸�������....

4.���´����
./bin/repack-bootimg.sh ./tmp/boot.img-kernel.gz ./tmp/boot.img-ramdisk ./myboot.img
