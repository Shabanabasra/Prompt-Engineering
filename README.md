# Prompt-Engineering

Chain-of-thought-Tree-of-Thought-self-consistency-and-React
                                                 
                                                                   Chain-of-Thought
                                                  
Chain-of-thought reasoning breaks complex problems into a clear sequence of intermediate steps so both humans and models can follow the logic from premise to conclusion. This approach improves transparency and correctness—e.g., instead of outputting “42,” a model shows the arithmetic steps (12 × 3 + 6 = 42), which makes it easier to verify, debug, and trust the result.
Example: Instead of saying “The answer is 42,” a model using chain-of-thought would show: “First, multiply 12 × 3 = 36. Then add 6 → 42.” This makes reasoning transparent, interpretable, and verifiable — especially useful in coding, math, and decision-making tasks.
                                                                    Tree-of-Thought
                                                    
Tree-of-thought expands single linear reasoning into a branching search that explores multiple alternative reasoning paths in parallel, pruning dead-ends and amplifying promising directions. It’s like sketching multiple solution routes on a whiteboard—useful in design or planning tasks (e.g., brainstorming product features where each branch represents a different user persona and implementation trade-offs).
Example: When planning a product launch, an AI might explore three branches: (1) Social media campaign, (2) Influencer marketing, (3) Email automation. It evaluates each branch, prunes weak ideas, and picks the most promising path. This mirrors how strategic thinkers evaluate options before acting.
                                                                    Self-Consistency
                                                        
Self-consistency boosts reliability by sampling many independent reasoning traces and picking the most consistent answer (majority vote) rather than trusting a single run. For instance, when answering a tricky logic puzzle, you generate several solution paths and choose the answer that appears most often across runs, reducing the chance of a fluke error from one mistaken chain.
Example: If an AI solves a riddle five times and four answers say “Paris” while one says “London,” the model will choose “Paris.” This “majority reasoning” ensures stability and confidence in complex or ambiguous problems.
                                                                  ReAct (Reasoning + Acting)
                                                  
ReAct combines step-by-step reasoning with explicit actions in the environment—like querying a database, invoking a calculator, or calling a search tool—so the agent reasons, acts, observes, and adapts in a loop. Practically, this looks like: “I should search the docs → (action: search) → found example code → (reason) integrate snippet,” which is powerful for tasks that require both thinking and doing (debugging, research, or multi-step automation).
Example :“To find the current Bitcoin price, I’ll (1) reason: I need live data → (2) act: call the CoinLayer API → (3) reason: interpret response → (4) answer: $68,000.” This loop of reasoning and action makes ReAct ideal for research agents, AI assistants, and automation workflows.

