# webscraping-ai-solution


Problems
1. The web is full of quality structured data, many developers are in the process of building knowledge bases to build AI tools but there is no turn-key way to get the structured data automatically.
2. The web is full of quality unstructured data but typically a human in the loop (manually or with custom parsers) has been required to parse into structured data.
3. Anti-bot / Anti scrapers are becoming more common for both public and private data, fully integrated captcha and proxy networking is required.

Existing AI parse tools
1. Diffbot
2. Zyte

Use Case #1
Automatically define python parser to use for given website. This is more suited for large crawls of one website. For example a knowledge base where the page structure is always the same for Apple IPhone Support

1. Identify arbitrary metadata for extraction via python parser: title, author, category, tags. Its important that this set is done in the parse stage because it doesnt require chatgpt for generation.
2. If unable to parse, return unstructured parsed text from beautiful soup

Solution
1. Use Scrapy or Crawlee to crawl with a proxy network
2. Use combination of chat gpt and beautiful soup to write initial parser
3. Classify or evaluate if the parser was a success, if not, write a new one with chat gpt
 
