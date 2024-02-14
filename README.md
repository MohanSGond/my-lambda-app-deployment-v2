# My Lambda App

This is a simple AWS Lambda application written in Node.js. It is deployed using the Serverless Framework and GitHub Actions.

## Project Structure

- `src/handler.js`: Contains the AWS Lambda handler function.
- `src/utils/index.js`: Exports utility functions used throughout the application.
- `src/tests/handler.test.js`: Contains tests for the `handler.js` file.
- `serverless.yml`: Configuration file for the Serverless Framework.
- `package.json`: Configuration file for npm.

## Setup

1. Install dependencies: Run `npm install` in the project root.
2. Set up AWS credentials: Configure your AWS credentials as per the Serverless Framework [documentation](https://www.serverless.com/framework/docs/providers/aws/guide/credentials/).
3. Deploy: Run `npx serverless deploy` to deploy the application to AWS Lambda.

## GitHub Actions

The GitHub Actions workflow is defined in `.github/workflows/main.yml`. It runs on the `windows-latest` environment and deploys the application using `npx serverless deploy`.

## Testing

Run `npm test` to execute the tests located in `src/tests`.

## Contributing

Please read `CONTRIBUTING.md` for details on our code of conduct, and the process for submitting pull requests to us.

## License

This project is licensed under the MIT License - see the `LICENSE.md` file for details.