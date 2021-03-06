# CommandLines

1- Append text into file without open it 
```Shell 
echo "Add your text here" >> filename.extension
```


2- Move file into another directory
```Shell 
mv "file path" "directory path"
```


3- Open home directory
```Shell 
open $HOME
```

4- Change your user password
```Shell 
passwd
```

5- Print string with more than one lines
```Shell 
cat <<-EOF
 "Add here your test with any number of lines"
EOF
```

6- Open Xcode archive folder
```Shell 
open ~/Library/Developer/Xcode/Archives
```

7- Add you repo as your submodule in git
```Shell 
git submodule add git@github.com:username/reponame.git
```

8- The first time you checkout a submodule repo
```Shell 
git submodule update --init --recursive
```

9- When need to pull a submodule repo
```Shell 
git submodule update --recursive --remote
```

10- Close all Xcode simulators
```Shell 
sudo killall -9 com.apple.CoreSimulator.CoreSimulatorService
```

11- Compress PDF
```Shell 
brew install ghostscript

gs -sDEVICE=pdfwrite -dCompatibilityLevel=1.4  -dPDFSETTINGS=/ebook -dNOPAUSE -dQUIET -dBATCH -sOutputFile=/inputPath /outputPath

```

12- Take Simulator ScreenShot
```Shell 
xcrun simctl io booted screenshot <filename>.<file extension>

After finish:
Ctrl + C
```

13- Record Simulator Video
```Shell 
xcrun simctl io booted recordVideo <filename>.<file extension>

After finish:
Ctrl + C
```

14- Merge one commit from branch to another
```Shell 
git cherry-pick <commit>
```

15 - Get branch's SHA1
```Shell
git rev-parse Branch name
```

16- Revert merged branch
```Shell
git revert -m 1 branch's SHA1
```

17- show hidden files mac
```Shell
defaults write com.apple.finder AppleShowAllFiles YES
killall Finder
```

18- Rollback to specific history of file in git
```Shell
git checkout "hash of the commit which has that veriosn of the file" "file1/to/restore file2/to/restore"
```

19- Set ssh password 
```Shell
cd ~/.ssh/; ssh-add
```

20- Clear Xcode simulators 
```Shell
xcrun simctl erase all
```

21- Abort git Rebase
```Shell
git rebase --abort
```

22- Update Cocoapods [Read more](https://1upnote.me/post/2018/06/updating-cocoapods-latest-version/)
```Shell
sudo gem install cocoapods
```
or 
```Shell
sudo gem install -n /usr/local/bin cocoapods
```

23- Update Cocoapods with pre releases [Read more](https://1upnote.me/post/2018/06/updating-cocoapods-latest-version/)
```Shell
sudo gem install cocoapods --pre
```

24- Show the duration of builds in Xcode
```Shell
defaults write com.apple.dt.Xcode ShowBuildOperationDuration -bool YES
```
