# Welcome to Persian Subtitle Fixer
A Bash script to change the unicode of Farsi/Persian subtitle to UTF-8 unicode. 

این برنامه برای مشکل انکودینگ زیرنویس های فارسی ساخته شده است. نحوه استفاده در ادامه توضیح داده شده است

# Dependencies 
* moreutils 

For Ubuntu Fans : 

`# apt-get install moreutils`

For Fedora Fans : 

`# dnf install moreutils`

Other RedHat based OSs: 

`# yum install moreutils`
# Download or Clone
Now download sub-fixer and change the premission by below command: 

`chmod 755 sub-fixer`

Now, Everything is ready !
# How to use this script ?
Actually there is two way : 
* *First Way*  fix all subtitle in your directory , `cd` to your specific directory you want and execute sub-fixer without any parameter:

 `$ sub-fixer `


##Example: 
```
cd Downloads/Batman-vs-Superman/
ls 
batman-480.srt batman-720.srt batman-1080.srt
sub-fixer  

```
sub-fixer start search for all srt files and check if they are n't utf-8 encode change them to utf-8

***
 
* *Second Way* , execute command for specific subtile : 

 `$ sub-fixer [Name-of-Your-Subtile]` 

## Example: 
```
cd Download/Batman-vs-Superman/
sub-fixer batman-1080.srt
```
