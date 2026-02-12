# Linux
Linux Troubleshootings


ls -la /home/csd-admin/
You should see:

.bash_profile
.bashrc
If missing → create basic one:

echo 'export PS1="[\u@\h \W]\\$ "' >> ~/.bashrc
source ~/.bashrc


[root@caasafq1-ncsafq1-genricedg1n-0 ~]# su csd-admin 
bash-4.4$ ls -la /home/csd-admin/
total 24
drwx------.  4 csd-admin admin    55 Jan 21 14:06 .
drwxr-xr-x. 16 root      root    256 Mar 24  2025 ..
drwx------.  3 csd-admin admin    17 Jan 21 14:06 .ansible
-rw-------.  1 csd-admin admin 22565 Feb 12 17:13 .bash_history
drwx------.  2 csd-admin admin    48 Feb  9 14:28 .ssh
bash-4.4$ echo 'export PS1="[\u@\h \W]\\$ "' >> ~/.bashrc
bash-4.4$ source ~/.bashrc
[csd-admin@caasafq1-ncsafq1-genricedg1n-0 root]$ 


solve it 
