# Parser
The current solution uses a using a smart combo of:

1. Pattern recognition (with regex)

2. Semantic search (powered by BERT)

3. Context-aware logic

## This is how the logic works:
1. It understands the layout by first reading each page of the PDF.

2. The entire text is broken down into sentences and chekcked cross checked for headings like “Management” or “Fund Summary”. 

3. Such sentences are filtered for important keywords and financial data .

4. Then it uses BERT embeddings to understand context better—for example, figuring out if “BlackRock” is acting as a sponsor or just mentioned in passing.

5. Finally, it pulls out the best matches and gives them to you—plus a list of any assumptions it made along the way.

## Can this scale?

We can modify the logic to run over multiple pdf files instead of just one. We can also extend the keywords and the rules set for pattern field_contexts to work for other fund types.

This definitely needs a lot of work but we can slowly get there by further fine tuning the logic and pattern or using a different more powerful model after research. 



   

