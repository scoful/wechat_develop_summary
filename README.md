# 基于微信体系开发的一些总结
包括服务号h5开发、小程序开发。


## 目录：

### [1.微信开发前置知识准备](./微信开发前置知识准备.md)
### [2. 微信各种号的区别与联系](./微信各种号的区别与联系.md)
### [3. 微信发消息能力总结](./微信发消息能力总结.md)
### [4. 微信开发中可能遇到的坑](./微信开发中可能遇到的坑.md)



<table class="table table-bordered table-hover table-condensed">
<thead><tr><th title="Field #1">FIELD1</th>
<th title="Field #2">服务号</th>
<th title="Field #3">小程序</th>
</tr></thead>
<tbody><tr>
<td>通过openId发送</td>
<td>Y</td>
<td>Y</td>
</tr>
<tr>
<td>推送位置</td>
<td>服务号对话框</td>
<td>服务通知</td>
</tr>
<tr>
<td>需要有交互</td>
<td>N</td>
<td>Y</td>
</tr>
<tr>
<td>交互动作是</td>
<td>-</td>
<td>支付(prepay_id)，提交表单(formId)</td>
</tr>
<tr>
<td>发送时间限制</td>
<td>不限制</td>
<td>7天内</td>
</tr>
<tr>
<td>发送数量限制</td>
<td>只受限于每日接口调用量：10W/100W/1000W，目前是100W，随着粉丝数正向增加</td>
<td>1个prepay_id7天内可发3条，1个formId7天内可发1条，目前默认每个账号日调用限额100W</td>
</tr>
<tr>
<td>可使用模板总数</td>
<td>25</td>
<td>25</td>
</tr>
<tr>
<td>行业限制</td>
<td>可选2个行业，每月可修改1次</td>
<td>暂无发现</td>
</tr>
<tr>
<td>跳转URL</td>
<td>支持，海外账号没有跳转能力，不填不跳转</td>
<td>不支持</td>
</tr>
<tr>
<td>跳转小程序</td>
<td>支持，发模板消息服务号必须与小程序是绑定关联关系，可跳到小程序的具体页面路径，可带参数，不支持小游戏，不填不跳转</td>
<td>支持，可跳到小程序的具体页面路径，可带参数，不填不跳转</td>
</tr>
<tr>
<td>修改内容能力</td>
<td>支持，可修改模板内容字体颜色，不填默认为黑色</td>
<td>支持，可放大某个关键词</td>
</tr>
</tbody></table>
