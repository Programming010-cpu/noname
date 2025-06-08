# 附录D：结束阶段摸牌技能示例

一个最基础的触发技，在你的回合结束阶段触发，你可以选择摸一张牌。

```javascript
"ex_end_draw": {
    trigger: { player: "phaseEnd" },
    prompt: "你可以摸一张牌",
    async content(event, trigger, player){
        await player.draw();
    }
} // 结束阶段，你可以摸一张牌
```
