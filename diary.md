[2023-01-30 16:08:55] <details> <summary>github个人主页图标</summary>
<p align="center">
	<img title="Hadoop" alt="Hadoop" src="https://raw.githubusercontent.com/Thomas-George-T/Thomas-George-T/master/assets/hadoop.svg" width="70" height="40" style="vertical-align:down; margin:4px"/>
	<img title="Spark" alt="Spark" src="https://raw.githubusercontent.com/Thomas-George-T/Thomas-George-T/master/assets/apache_spark.svg" width="80" height="50" style="vertical-align:down; margin:4px"/>
	<img title="AWS" alt="AWS" src="https://raw.githubusercontent.com/Thomas-George-T/Thomas-George-T/master/assets/aws.svg" width="60" height="40" style="vertical-align:down; margin:4px"/>
	<img title="Scala" alt="Scala" src="https://raw.githubusercontent.com/Thomas-George-T/Thomas-George-T/master/assets/scala.svg" width="40" height="40" style="vertical-align:down; margin:4px"/>
	<img title="Python" alt="Python" src="https://raw.githubusercontent.com/Thomas-George-T/Thomas-George-T/master/assets/python.svg" width="40" height="40" style="vertical-align:down; margin:4px"/>
	<img title="R" alt="linux" src="https://raw.githubusercontent.com/Thomas-George-T/Thomas-George-T/master/assets/r-lang.svg" width="55" style="vertical-align:down; margin:4px"/>
	<img title="MySQL" alt="MySQL" src="https://raw.githubusercontent.com/Thomas-George-T/Thomas-George-T/master/assets/mysql.svg" width="40" height="40" style="vertical-align:down; margin:4px"/>
	<img title="Bitbucket" alt="Bitbucket" src="https://raw.githubusercontent.com/Thomas-George-T/Thomas-George-T/master/assets/bitbucket.svg" height="40" style="vertical-align:down; margin:4px"/>
	<img title="Git" alt="Git" src="https://raw.githubusercontent.com/Thomas-George-T/Thomas-George-T/master/assets/git.svg" width="70" height="40" style="vertical-align:down; margin:4px"/>
	<img title="Bamboo" alt="Bamboo" src="https://raw.githubusercontent.com/Thomas-George-T/Thomas-George-T/master/assets/bamboo.svg" width="40" height="40" style="vertical-align:down; margin:4px"/>	
	<img title="jira" alt="linux" src="https://raw.githubusercontent.com/Thomas-George-T/Thomas-George-T/master/assets/jira.svg" width="40" style="vertical-align:down; margin:4px"/>
	<img title="Kafka" alt="Kafka" src="https://raw.githubusercontent.com/Thomas-George-T/Thomas-George-T/master/assets/kafka.svg" width="105" height="40" />
	<img title="linux" alt="linux" src="https://raw.githubusercontent.com/Thomas-George-T/Thomas-George-T/master/assets/linux-tux.svg" width="40" style="vertical-align:down; margin:4px"/>	
	<img title="Tableau" alt="Tableau" src="https://raw.githubusercontent.com/Thomas-George-T/Thomas-George-T/master/assets/tableau.svg" width="200" style="vertical-align:down; margin:4px"/>
</p>
</details>
[2023-01-30 19:57:31] 

### CMD常用命令 
* e: 进入E盘
* mkdir 在当前目录创建多级目录 只能创建文件夹
* type nul>1.txt 在当前目录添加txt空文件, 可自定义后缀名
* pushd 堆栈底部 popd从上面蹦出来 形象 使用失败


[2023-01-31 02:37:28]

<details><summary> Github Action 错误403 权限错误搞不懂 搞了一天还是搞不出来 索性手动操作了</summary>
<p align= "center">

```
# GitHub Action for generating a contribution graph with a snake eating your contributions.

name: Generate Snake

on:
  schedule:
    - cron: "0 0 * * *"
  workflow_dispatch:

jobs:
  build:
    runs-on: ubuntu-latest

    steps:
      - name: Checkout
        uses: actions/checkout@v2.3.4
      
      - name: Generate Snake
        uses: Platane/snk@master
        id: snake-gif
        with:
          github_user_name: ${{ github.repository_owner }}
          gif_out_path: ./assets/github-contribution-grid-snake.gif
          svg_out_path: ./assets/github-contribution-grid-snake.svg

      - name: Push to GitHub
        uses: EndBug/add-and-commit@v7.2.1
        with:
          branch: main
          message: 'Generate Contribution Snake'
```
</p>
</details>