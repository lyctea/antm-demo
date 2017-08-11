# [Ant Design Mobile of React][1]

[1]:[https://mobile.ant.design/docs/react/introduce-cn]

尝试使用Ant Design Mobile组件。

尝试在找到移动端适配的更好的方案。

# 项目配置

## 使用create-react-app 脚手架
在此基础上的必要设置：
- 入口页面必需的设置：

- 引入『高清方案』设置：具体方法见 wiki 里 antd-mobile-0.8-以上版本「高清」方案设置。

- 引入 FastClick, 关联 #576

- 引入 Promise 的 fallback 支持 (部分安卓手机不支持 Promise)，示例代码如：

`
if(!window.Promise) {
  document.writeln('<script src="https://as.alipayobjects.com/g/component/es6-promise/3.2.2/es6-promise.min.js"'+'>'+'<'+'/'+'script>');
}
`

具体参考 [在 create-react(-native)-app 中使用][2]

[2]:[https://mobile.ant.design/docs/react/use-with-create-react-app-cn]

# 组件使用

项目中需要提前做一些配置工作，按需引入，图标等
具体参考 [Web 使用方式][3]

[3]:[https://mobile.ant.design/docs/react/introduce-cn]

`
// Auto import js and css modularly, parsed by babel-plugin-import
import { Button } from 'antd-mobile';
ReactDOM.render(<Button>Start</Button>, mountNode);
`

