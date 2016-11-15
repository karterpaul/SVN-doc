* repo creation
svnadmin create /home/mysurface/repo/programming_repo



*check out
sudo svn checkout svn+ssh://karter@192.168.3.240/usr/local/svn/repos/test test
*branching
svn copy svn+ssh://host.example.com/repos/project/trunk \
           svn+ssh://host.example.com/repos/project/branches/NAME_OF_BRANCH \
      -m "Creating a branch of project"

* update
sudo svn update


*merging

/svnrepo/test/branch/newbr$ sudo svn merge /home/karter/svnrepo/test/trunk


*status
~/svnrepo/test/branch/newbr$ sudo svn status



chenge truvk to brach

~/svnrepo/test/trunk$ sudo svn merge --reintegrate /home/karter/svnrepo/test/branch/newbr
	
*delete branch

svn delete ^/calc/branches/my-calc-branch \



*reference
http://svnbook.red-bean.com/en/1.7/svn.branchmerge.using.html


user to svn group







=================
svn copy svn+ssh://192.168.3.240/usr/local/svn/repos/test/trunk svn+ssh://192.168.3.240/usr/local/svn/repos/test/branch/br001

//192.168.3.240/usr/local/svn/repos/wservice

wget http://server.com/svn/trunk/test.file for getiing single file from repository
and the apply svn update



user creation for svn and ssh


sudo adduser username  	

adding user to svn group

sudo usermod -a -G groupName userName




