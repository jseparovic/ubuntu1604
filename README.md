### Build steps
apt update -y
apt install build-essential dh-autoreconf libcurl4-gnutls-dev libexpat1-dev gettext libz-dev libssl-dev -y
apt install -y cmake libcap-dev libbz2-dev libclang-dev
wget http://archive.ubuntu.com/ubuntu/pool/main/c/cdrkit/cdrkit_1.1.11.orig.tar.gz
tar xfvz cdrkit_1.1.11.orig.tar.gz
cd cdrkit-1.1.11/
make

### Build Machine
root@ubuntu-2gb-hil-1:~# cat /etc/os-release
NAME="Ubuntu"
VERSION="20.04.6 LTS (Focal Fossa)"
ID=ubuntu
ID_LIKE=debian
PRETTY_NAME="Ubuntu 20.04.6 LTS"
VERSION_ID="20.04"
HOME_URL="https://www.ubuntu.com/"
SUPPORT_URL="https://help.ubuntu.com/"
BUG_REPORT_URL="https://bugs.launchpad.net/ubuntu/"
PRIVACY_POLICY_URL="https://www.ubuntu.com/legal/terms-and-policies/privacy-policy"
VERSION_CODENAME=focal
UBUNTU_CODENAME=focal

root@ubuntu-2gb-hil-1:~# uname -a
Linux ubuntu-2gb-hil-1 5.4.0-144-generic #161-Ubuntu SMP Fri Feb 3 14:49:04 UTC 2023 x86_64 x86_64 x86_64 GNU/Linux
