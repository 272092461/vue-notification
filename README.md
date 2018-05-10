# vue-notification 扩展

github: https://github.com/272092461/vue-notification

## vue-notification

github: https://github.com/euvl/vue-notification

## notification左侧允许显示自定义图片

```javascript
this.$notify({
  group: 'foo',
  image: '/images/example.jpg',
  title: 'Important message',
  text: 'Hello user! This is a notification!'
});
```

## notification 点击回调

```html
<notification @itemclick="callback"></notifaction>
```

## 为点击回调提供参数

```javascript
  // 调用参数
  this.$notify({
    group: 'foo',
    image: '/images/example.jpg',
    title: 'Important message',
    text: 'Hello user! This is a notification!',
    // 该属性只用于回调参数
    mark: {
      id: '...'
    }
  });

  new Vue ({
    methods: {
      callback: function (item) {
        console.log(item.title)
        console.log(item.text)
        console.log(item.mark)
      }
    }
  })
```

## 更多API

github: https://github.com/euvl/vue-notification