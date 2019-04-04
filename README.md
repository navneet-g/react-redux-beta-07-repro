How to repro
1) Clone this repo
2) yarn
3) npm run start
4) Launch the redux dev tools
5) Click on hacker news checkbox
6) Dispatch following actions using redux dev tools, notice that the hacker noon widget updates only after dispatching twice, you can keep changing title below to see the updates to widgets are one step behind

```
{
  type: 'hackernews/storiesavailable',
  payload: {
    items: [
      {
        by: 'openbasic',
        descendants: 48,
        id: 19567160,
        kids: [
          19567656,
          19568134,
          19567481,
          19567794,
          19567490,
          19567615,
          19567697,
          19567466
        ],
        score: 119,
        time: 1554324579,
        title: 'The Lobster2 Programming Language',
        type: 'story',
        url: 'http://strlen.com/lobster/'
      }
    ]
  }
}
```