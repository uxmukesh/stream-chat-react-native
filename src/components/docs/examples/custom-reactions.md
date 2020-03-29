# Message with custom reactions

`MessageSimple` accepts a prop - `supportedReactions`. You can pass your emoji data to this prop to set your own reactions.

In this example I will support only two reactions - Monkey face (🐵) and Lion (🦁)

```js
const MessageSimpleWithCustomReactions = (props) => (
    <MessageSimple
      {...props}
      supportedReactions={[
        {
          id: 'monkey',
          icon: '🐵',
        },
        {
          id: 'lion',
          icon: '🦁',
        },
      ]}
    />
  );
```