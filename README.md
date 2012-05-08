# code_swarm video generator

This script helps to generate a svn repository's activity video based on code_swarm software.

This script has been tested on Debian but should work on Ubuntu.

Example:
<code>
./code_swarm-video-generator --output=./subversion-project.avi --fpd=10 --svn-range=HEAD:1300000 http://svn.apache.org/repos/asf/subversion/trunk/
</code>

It will produce this video:
https://github.com/kerphi/code_swarm-video-generator/raw/master/subversion-project.avi