# 周会分享

分享项目管理流程

## 项目管理流程

### 1.流程

项目的主要流程是：预立项阶段-执行阶段-线上运营阶段。

1.产品：[需求分析] - `需求评审` - `高保真评审` - 产品验收 - {产品迭代} - {产品运营}

2.质量：[测试方案设计] - `测试用例评审` - 集成测试 - 测试报告 - {测试迭代}

3.研发：[技术预研/原型验证] - `方案设计评审` - 开发 - 提交测试 - 修复改进 - `上线评审` - {研发迭代}

### 2.预立项阶段

1.申请预立项：判断项目合理性，项目成果是否和产品需求一致，人力分配合理性

2.阶段工作:组织人员调研，准备立项评审材料，项目经理跟进进度

3.申请立项：编写立项报告，根据实际情况给出合适的Demo，说明目前可以达到的效果

4.立项通过标准：需求方案、技术方案、工作计划

### 3.项目执行阶段

执行阶段由子项目负责人对项目负责，带领项目参与人员按计划开展项目研发，按目标完成项目的研发达到上线运营要求。主项目的项目经理可对子项目进行指导和监督。

1.子项目由项目负责人负责进行推进，对过程进行风险管控。

2.产品进行需求分析，提交原型和PRD，并组织需求相关人员进行评审，评审通过后，进入UI设计阶段，需求评审不通过，则结合评审意见继续修改

3.UI设计完，UI组织需求相关人员评审，评审通过后进入API接口及方案设计阶段，评审不通过，则结合评审意见继续修改

4.开发提交接口定义，前端以及测试确认API接口无误后，测试编写接口测试用例。否则，开发结合双方意见继续修改

5.后端开发至少提前3天交付接口，并自测通过，研发确认交付,确认不通过，则继续修改

6.开发前后端联调自测通过后，根据时间计划，统一提交QA冒烟测试，否则继续修改

7.QA冒烟测试通过后，进入测试阶段，否则，开发继续修改自测，再次提交冒烟测试

8.QA提交问题，开发修改问题，修改完成后，进入回归测试

9.QA验证问题，验证完毕后，进入上线发版阶段，项目管理创建发版issue，并验证功能

10产品负责在RC环境验证功能

#### 3.1 测试工作

1.第一轮测试：执行所有测试用例，提交问题单，开发解决所有1、2级bug和90%3、4级bug。开发提交代码，测试转入dev分支

2.dev测试：在dev分支进行回归测试，验证通过所有非确认遗留bug，测试转入release分支

3.RC测试：回归测试所有问题单，产品验证通过，发布上线

#### 3.2 版本发布

1.上线评审：子项目负责人提交上线申请，测试提交测试报告，评审团（产品、项目管理、研发、QA、运维负责人）决定通过与否

2.运维负责人发布版本

3.测试线上验证，验证通过，产品验收，不通过回滚版本

4.产品验收通过，上线完成，推送最新版本给用户

5.项目经理进行迭代回溯，分析迭代问题和亮点

### 4.线上运营阶段

1.用户反馈处理：反馈内容、记录要求、处理后回复用户、把控进度

2.线上重大问题处理：遇到阻塞问题每两天同步进展、发布hotfix

