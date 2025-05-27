# metricalgpt

This repository explores tools for generating, scanning (parsing), and analyzing metrical lines (human and AI) 

You can:

1) generate prompts for metrical lines (prompt_generator.ipynb) + a few resulting dictionaries of prompts (prompts folder)

2) generate AI lines and parse these lines using prosodic.py (LLM_prompt_and_parse.ipynb)
   
   This takes dictionary of prompts, gets responses via API, then scans their meter

        Note: you will need api keys, but not many tokens for gemini-flash or 4o-latest
        
        Currently runs openai, see gemini_prompt_parse for gemini (buggy output right now)

3) tools for analyzing the results 
    parse_analysis/parse_df_analyzer.ipynb
    parse_analysis/prosodic_vs_metricalbert.ipynb [this compares a BERT classifier's guess about metrical complexity to actual parses]

Additionally, two other scansion scripts to let users try out prosodic.py on lines, texts, and corpora


    parseloop:  allows chunking and processing of larger csv corpora with prosodic.py


    easy_scansion_tool: to play with prosodic.py outputs and meter configurations 



## saved human corpora,  AI responses, and  analysis notebooks

AI data for o1_mini 

AI data for chatgpt-4o-latest (as of Jan 10 2025) 

AI data for gemini flash 1.5

[ECPA (Eighteen Century Poetry Archive)](https://www.eighteenthcenturypoetry.org/)

    filtered (basex / xqy) and cleaned to produce 18C blank verse lines and metrical analysis

    You can view and fetch this data (100k lines, parsed and scored) via huggingface: 
    https://huggingface.co/datasets/bensglaser/18C_IP_Scanned

       





