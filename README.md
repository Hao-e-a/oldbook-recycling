# oldbook-recycling
旧书回收系统
项目简介
旧书回收系统是一个面向学生和收书员的 Web 应用，旨在帮助学生处理不再需要的书籍。系统分为三大模块：学生、收书员 和 管理员。学生可以通过平台卖掉自己的旧书，或者寻找别人出售的旧书；收书员负责接单并回收书籍；管理员可以管理系统中的用户和审核书籍信息。

功能模块
1. 学生模块
注册和登录：使用学号注册，首次登录需要设置密码。
上传旧书：学生可以上传旧书的信息（书名、版次、封面等）和卖书的照片。
查找旧书：浏览其他学生上传的旧书，进行关键词搜索。
卖书：选择需要卖掉的书籍，上传书籍照片和描述。
收件箱：查看与其他学生的聊天记录，协调交易。
2. 收书员模块
接单：收书员可以浏览所在校区的待接单书籍，接取订单。
称量和收书：收书员到达学生宿舍后，称量书籍重量并记录。
付款：根据书籍重量计算回收费用，并将费用支付给学生。
3. 管理员模块
管理学生账户：管理员可以查看、禁用和删除学生账户。
审核书籍信息：审核学生上传的书籍信息，确保其真实性。
举报系统：学生和收书员可以举报违规行为，管理员会进行审核并做出相应的处理。
技术栈
前端：HTML, CSS, JavaScript
后端：Flask（Python）
数据库：SQLite
版本控制：Git，GitHub
部署平台：Heroku 或其他云平台
安装与运行
1. 克隆仓库
bash
复制
编辑
git clone https://github.com/yourusername/book_recycling.git
cd book_recycling
2. 创建虚拟环境并激活
bash
复制
编辑
python -m venv venv
source venv/bin/activate  # macOS/Linux
venv\Scripts\activate     # Windows
3. 安装依赖
bash
复制
编辑
pip install -r requirements.txt
4. 配置数据库
初始化数据库：

bash
复制
编辑
python create_db.py
5. 运行应用
bash
复制
编辑
python app.py
访问 http://127.0.0.1:5000 即可在本地查看系统。

功能展示
1. 学生注册和登录
学生在首次登录时，输入学号，并设置自己的密码。

2. 上传书籍
学生可以上传书籍信息，并添加书籍封面照片。

3. 收书员接单
收书员可以根据校区查看待回收的旧书，并接取订单。

4. 管理员后台管理
管理员可以管理学生账户，并审核学生上传的书籍信息。

项目结构
bash
复制
编辑
book_recycling/
├── static/
│   ├── css/
│   ├── js/
│   └── uploads/
├── templates/
│   ├── index.html
│   ├── login.html
│   └── ...
├── app.py
├── config.py
├── models.py
└── requirements.txt
说明：
static/：包含 CSS、JavaScript 和图片文件。
templates/：包含所有 HTML 模板文件。
app.py：Flask 主应用文件。
config.py：应用配置文件。
models.py：定义数据库模型。
requirements.txt：列出所有项目依赖的库。
贡献
欢迎任何人提交问题报告、建议和 PR。请遵循以下步骤来贡献代码：

Fork 本仓库。
创建一个新的分支 (git checkout -b feature-name)。
提交代码 (git commit -am 'Add feature-name')。
推送到分支 (git push origin feature-name)。
创建 PR。
License
MIT License
