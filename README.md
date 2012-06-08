# code_swarm video generator

This script helps to generate a svn repository's activity video based on code_swarm software.

This script has been tested on Debian but should work on Ubuntu.

Example:
<code>
./code_swarm-video-generator --output=./subversion-project.avi --fpd=10 --svn-range=HEAD:1300000 http://svn.apache.org/repos/asf/subversion/trunk/
</code>

It will produce this video:
https://github.com/kerphi/code_swarm-video-generator/raw/master/subversion-project.avi


## Options

    --svn-range: svn log range 
    --show-username: true or false, if true logins are displayed near the avatar
    --output: filename and path of the final video
    --fpd: frame per day (low number will make a fast video)
    --avatar-dir: absolute path where are located avatars
    --tmp-dir: absolute path for a temporary directory (used for internal work)

## Avatars

You can add avatars in the avatar/ folder. Each avatar should be 50x50 in PNG. The avatar's filename should be {login}.png where {login} is the name of the SVN login from the repository. If the image is not found, default.png will be used.