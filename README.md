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

12- Take ScreenShot
```Shell 
xcrun simctl io booted screenshot <filename>.<file extension>
```
