# otterbots-openAI

npm create vite@latest client --template vanilla
Select Vanilla framework
Select Javascript
cd client
npm install

Server Folder
npm install cors dotenv express nodemon openai
create .env in server folder and add the following line OPENAI_API_KEY = "your api-key"
https://platform.openai.com/account/api-keys -> create key and copy it into .env 

You can play around with these settings in server.js:

      temperature: 0, // Higher values means the model will take more risks.
      max_tokens: 3000, // The maximum number of tokens to generate in the completion. Most models have a context length of 2048 tokens (except for the newest models, which support 4096).
      top_p: 1, // alternative to sampling with temperature, called nucleus sampling
      frequency_penalty: 0.5, // Number between -2.0 and 2.0. Positive values penalize new tokens based on their existing frequency in the text so far, decreasing the model's likelihood to repeat the same line verbatim.
      presence_penalty: 0, // Number between -2.0 and 2.0. Positive values penalize new tokens based on whether they appear in the text so far, increasing the model's likelihood to talk about new topics.
