# ChatGPT Bash Script (`gpt`)
```
user:~$ gpt "Can you give me some dinner suggestions?"
Sure, here are a few dinner suggestions:

1. Grilled chicken or fish with roasted vegetables and baked sweet potato.
2. Quinoa and black bean bowl with avocado, salsa, and Greek yogurt drizzle.
3. Spinach and feta stuffed chicken breast with a side salad.
4. Lentil soup with crusty bread and a side of roasted asparagus.
5. Shrimp stir-fry with mixed vegetables and brown rice.
6. Grilled steak with sautéed mushrooms, garlic mashed potatoes and roasted carrots.
7. Cauliflower crust pizza with tomato sauce, mozzarella cheese, and vegetables like mushrooms, bell peppers, and onions.
8. Tofu or tempeh stir-fry with broccoli, bell peppers, carrots and brown rice.
9. Spaghetti with homemade marinara and meatballs.
10. Grilled salmon with roasted brussels sprouts and wild rice pilaf.
```

# Installation
1. Define a `OPENAI_API_KEY` environment variable with your OpenAI API key (https://platform.openai.com/account/api-keys).
2. Install `jq` (https://stedolan.github.io/jq/download/).
3. Download and use the `gpt` script.

# Usage
```
user:~$ gpt --help
Usage: gpt [...options] <question>
  -m, --model <model>     Set model to use, default is text-davinci-003 for 'text' completion and 
                          gpt-3.5-turbo for 'chat' completion. See 
                          https://beta.openai.com/docs/api-reference/models.
  -c, --completion_type <type>  Can either be 'chat' or 'text'. Default is 'text'.
  -t, --max_tokens <num>  Set the maximum number of tokens to generate in the completion. The token
                          count of your question plus max_tokens cannot exceed the model's context
                          length. Most models have a context length of 2048 tokens (except for
                          the newest models, which support 4096). Default is 4096 - question length.
  -h, --help              Display this help message.
```
