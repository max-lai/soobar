## 工作时间工具

以番茄时间管理法为基础，记录工作点滴。

```sql
CREATE TABLE `NewTable` (
`id`  int NOT NULL AUTO_INCREMENT ,
`content`  varchar(5000) NOT NULL DEFAULT 时间内容 ,
`src`  int NOT NULL DEFAULT 关联的原始事件 ,
`start_time`  timestamp NOT NULL DEFAULT 开始时间 ,
`end_time`  timestamp NOT NULL DEFAULT 结束时间 ,
`status`  tinyint NOT NULL DEFAULT 事件状态：0未开始 1部分完成 2全部完成 3暂停 4搁置 
PRIMARY KEY (`id`)
)
;
```

### 事件状态

+ 未开始
+ 部分完成 一个较大的事件拆分出来的
+ 全部完成
+ 暂停
+ 搁置