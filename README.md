# roadhogWebpack4
使用webpack4来代替roadhong，构建ant-pro项目，可以大幅度提高速度

# 接入方式
1. 将package.json中devDependencies中的依赖添加到自己的项目中，并删除项目中的roadhog依赖
2. 运行npm install 推荐使用(cnpm install速度更快,如果不知道自行百度cnpm)
3. 将.babelrc（babel配置）、.eslintrc（eslint配置）、.stylelintrc（stylelint配置）复制到项目根目录
4. 将config.dll.js（打包第三方依赖生成dll，不明白的自行去百度）、webpack.config.development.js（开发环境配置）、webpack.config.production.js（生产环境配置）复制到项目根目录
5. 运行buildDll 命令生成dll
6. 开发时运行start:local会启动webpack-dev-server 、开发环境打包运行webpack-build-development、生产环境打包运行webpack-build-production
