
### Running in a Docker container

1. **Obtaining Telegram api keys.**

Please visit this [page](https://github.com/telegramdesktop/tdesktop/blob/dev/docs/api_credentials.md) for details.

2. **Provide your Telegram api keys as build arguments.**

```bash
docker build . --build-arg TELEGRAM_API_ID=0000000 --build-arg TELEGRAM_API_HASH=00000000000000000 -t telegram_react
```
The Docker build will perform all the necessary steps to get a working build of Telegram-React.


3. running in container
```bash
docker run -e TELEGRAM_API_ID=0000000 -e TELEGRAM_API_HASH=00000000000000000 -p 3000:80 telegram_react
```



### References

1. [Deploying a React App (created using create-react-app) to GitHub Pages](https://github.com/gitname/react-gh-pages)
2. [Facebook's tutorial on deploying a React app to GitHub Pages](https://github.com/facebookincubator/create-react-app/blob/master/packages/react-scripts/template/README.md#github-pages)
