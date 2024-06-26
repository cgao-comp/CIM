该代码分两个部分，第一部分需要python运行的Node2vec部分，第二部分为matlab运行的算法主题部分，
其中Node2vec部分会将生成的先验信息保存到txt中，matlab运行时会读取该部分信息作为指导。

注意事项，
1. 本机运行环境为matlab r2016a，改代码需要适配对应版本globaloptim包（将其替换matlab\toolbox中的重名包）
2. 请自行调整python中与matlab中的文件保存路径（matlab文件路径在运行文件和create_populationLS中）
3. 示例代码中仅采用NMI指标（文件中有ARI），可根据输出和label格式自行添加及设计不同评估指标


运行：
1. 运行python文件获取先验信息，github上有不同实现的node2vec代码，请自行下载
2. 运行matlab中 run_MLMaOPmainsyn.m   更换数据集请 注释\取消注释 不同的代码块
3. 运行前需要在matlab左侧目录中把True及其子文件引入加入路径，matlab才能搜索到数据集


注1：snd数据集为样例，python中间结果已经拷贝到example_pre_extracted_prior_information中，直接运行即可，不需要运行python，其余数据集须调整路径
