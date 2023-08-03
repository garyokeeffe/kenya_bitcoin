# Kenya Bitcoin AI
Most Bitcion content is produced for English speaking westerners. Even if we could translate this content into Swahili, most of it wouldn't appeal to a person in East Africa.

This is a Swahili-first Bitcoin education chatbot that layers Kenyan and Tanzanian cultural context into how it delivers it's responses to users. It's aim is to facilitate self-directed and self-paced Bitcion education for the ~130 million natvie Swahili speakers in East Africa. 

## Technical Development
[Master Guantai]("https://twitter.com/MasterGuantai")---a Bitcoin Educator living in Nairobi, Kenya---was the main prompt engineer on this project. He optimized an open source [ Bitcoin-aligned Chat GPT prompt]("https://github.com/garyokeeffe/chatBTC") to perform well in East Africa by fusing it with cultural elements from Tanzania and Kenya.

The front-end is a modified [Chatbot-UI]("https://github.com/mckaywrigley/chatbot-ui") interface. It was initially modified to provide Master Guantai with a prompt engineering environment wherein he could get a feel for how his tweaks to the prompts would change model output. Once we finalized a well-performing prompt, we modified the front-end further, stripping it back to provide the user with a simple interface.

## Performance
This chatbot's performance has not yet gone through rigourous assessment. However, we have two sources of leading indication.

Firstly, and anecdotally, Master Guantai distributed the chatbot to several Bitcoiners in Kenya and instructed them to try and break it. This process was overwhelmingly successful---most people were unsuccessful in their efforts, but some were successful, and as a result the chatbot is more robust in answering questions around Bitcion and halal.

Secondly, and quantatively, the [Bitcoin-aligned Chat GPT prompt]("https://github.com/garyokeeffe/chatBTC") that was used as the basis of Master Guantai's prompt engineering was benchmarked in May 2023 and performed 16% better than GPT-3.5 at answering Bitcion related questions. However in specific subcategories (such as Bitcion vs Crypto) the Bitcoin-aligned prompt outperformed vanilla GPT-3.5 by 100% (see figure below for more details on benchmarking).

![LLM Benchmark](https://github.com/garyokeeffe/kenya_bitcoin/blob/main/BitcoinLLMUpdate1.png)

## Future work
Next steps for this project are:
- add ability to record user interactions so that we can understand and report on common lines of questioning
- formally release this project into the world
- add other languages (and cultural contexts) to the chatbot
- share our processes, tools, and insights with other like-minded individuals on similar missions