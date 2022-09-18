# Git

## HEAD
به ما نشان میدهد در کجا قرار داریم

## Remote
دستور git remote امکان ایجاد، مشاهده و حذف ارتباط با مخزن های دیگر را به شما می دهد. اتصال های از راه دور بیشتر شبیه نشانه گذاری (bookmark) ها هستند تا لینک مستقیم به مخزن های دیگر. آن ها به جای دسترسی سریع (real-time)به مخزن دیگر، به عنوان نام های مناسبی هستند که می توانند برای آدرس (URL) های نه چندان خوانا باشند.  

دستور زیر لیست اتصال های از راه دور را فهرست می کند. 
``` bash
git remote
```
این دستور مانند دستور بالا است، اما آدرس هر اتصال را نیز در خروجی نمایش می دهد.

``` bash
git remote add <name> <url>
```
با استفاده از دستور بالا، اتصال جدیدی به یک مخزن از راه دور ایجاد کنید. پس از افزودن یک اتصال از راه دور، می توانید به عنوان میانبر مناسب برای سایر دستورهای Git استفاده کنید.


``` bash
git remote rm <name>
```
اتصال به مخزن از راه دور را حذف کنید.

``` bash
git remote rename <old-name> <new-name>
```
نام اتصال از راه دور را به نام جدید تغییر دهید. 


## Merge
دستور git merge چندین commit را به یک تاریخچه ی واحد متصل می کند.
<br>
مثال:
```bash
# Start a new feature
git checkout -b new-feature main
# Edit some files
git add <file>
git commit -m "Start a feature"
# Edit some files
git add <file>
git commit -m "Finish a feature"
# Merge in the new-feature branch
git checkout main
git merge new-feature
git branch -d new-feature
```
## Rebase
``` bash
git rebase -m "initail"
```
## Revert
## Cherry Pick
## Pull Request
## Submodules
## Reset
## Working area VS Staging area
## bisect
