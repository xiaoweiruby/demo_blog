# Let's Build: With Ruby On Rails - Blog With Comments

## 案例分析：

### 构建 demo_blog 的案例的关键在于完成三个维度的动作：

- （1） gem 安装和调试；
- （2） 增删改查 的功能的调试 + 样式 的调试；
- （3） 评论功能 的调试；

```
cd workspace
rails new demo_blog
ls
cd demo_blog
ls
git init
git status
git add .
git commit -m "initial commit"
rails server
git remote add origin https://github.com/shenzhoudance/demo_blog.git
git push -u origin master
```
![image](https://ws4.sinaimg.cn/large/006tNc79gy1fpre75f7c0j317w0me0yi.jpg)
![image](https://ws1.sinaimg.cn/large/006tNc79gy1fpre47c21ej31040y0az2.jpg)

```
git checkout -b gem
https://rubygems.org/
gem 'better_errors', '~> 2.4'
gem 'bulma-rails', '~> 0.6.2'
gem 'simple_form', '~> 3.5', '>= 3.5.1'
---
group :development do
---
gem 'guard', '~> 2.14', '>= 2.14.2'
gem 'guard-livereload', '~> 2.5', '>= 2.5.2'
---
bundle install
git add .
git commit -m "add gems"
```
https://bulma.io/documentation/overview/start/
https://github.com/guard/guard-livereload
http://livereload.com/extensions/
```
rails generate simple_form:install
gem 'guard-livereload', '~> 2.5', '>= 2.5.2', require: false
bundle
rails s
bundle exec guard
exit
```
![image](https://ws2.sinaimg.cn/large/006tNc79ly1fpsbhgsktij313207wmza.jpg)
![image](https://ws4.sinaimg.cn/large/006tNc79ly1fpsbfs8wjmj31kw0p87d6.jpg)
![image](https://ws4.sinaimg.cn/large/006tNc79ly1fpsbgpxuv6j31hw0rq45t.jpg)

git status
git add .
git commit -m "add gems"
git push origin gem
