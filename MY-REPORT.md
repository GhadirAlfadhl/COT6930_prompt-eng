![GenI-Banner](https://github.com/genilab-fau/genial-fau.github.io/blob/8f1a2d3523f879e1082918c7bba19553cb6e7212/images/geni-lab-banner.png?raw=true)

#  Evaluating Prompt Engineering Techniques for a Cybersecurity AI Study Companion

An AI-powered Discord study companion that assists students with Cybersecurity through scenario-based problem-solving, real-world examples, interactive assessments, and dynamic explanations.


* Authors: [Ghadir Alfadhl](https://github.com/GhadirAlfadhl)
* Academic Supervisor: [Dr. Fernando Koch](http://www.fernandokoch.me)

  
# Research Question 

Investigating the effectiveness of various prompt engineering strategies to determine the best methods for designing a responsive AI study companion that enhances cybersecurity education through interactive learning and real-time support.

## Arguments

#### What is already known about this topic

* Prompt engineering is key in customizing AI behavior for domain-specific applications like cybersecurity.
* Slight variations in prompt formulation can lead to markedly different AI responses in terms of accuracy, depth, and engagement.
* You could implement structured prompt experimentation to refine AI performance in handling cybersecurity content.
* The possibility of automating prompt optimization using reinforcement learning or fine-tuning with user feedback is promising.
* Challenges include maintaining contextual integrity across multi-turn interactions and mitigating hallucinations in technical explanations.

#### What this research is exploring

* We employ different prompt engineering methods (e.g., few-shot, chain-of-thought, role-based prompting) to evaluate their performance in delivering accurate, context-sensitive cybersecurity responses.
* We are building a Discord-based AI chatbot tailored to help students learn foundational and advanced cybersecurity concepts.
* We are exploring adaptive prompt strategies that evolve based on interaction data and learning progression.

#### Implications for practice

* It will be easier to provide real-time cybersecurity tutoring and practice scenarios through AI.
* It will optimize how students interact with technical content by offering scaffolded assistance and tailored explanations.
* We will better understand how to fine-tune AI assistants for technical domains, enhancing digital learning tools in cybersecurity education.


# Research Method

This study follows a systematic approach involving iterative testing of different prompt engineering techniques to refine chatbot performance and enhance cybersecurity learning experiences.

## Defining the Scope and Objectives:

* Establish the primary goal of evaluating prompt engineering techniques for an AI-powered Discord companion focused on cybersecurity education.

* Set specific objectives: testing prompt structures, assessing response accuracy for technical tasks, and measuring student engagement.

## System Design and Development:

* Develop the Discord chatbot using Ollama and a chosen LLM (e.g., llama3 or GPT-4) to handle cybersecurity queries.

* Implement prompt engineering methods (zero-shot, few-shot, chain-of-thought) to examine their impact on response quality and technical correctness.

* Ensure the bot can simulate scenario-based problem-solving (e.g., threat modeling, encryption tasks) for diverse learner personas.

## User Interaction Testing:

* Conduct user testing with cybersecurity students to evaluate the chatbot’s ability to generate accurate, context-aware guidance.

* Compare interactions across different prompt strategies to identify which methods improve comprehension and practical application.

* Implement A/B testing to analyze variations in effectiveness based on prompt modifications.


## Iterative Refinement:

* Refine prompt templates based on qualitative feedback and quantitative performance metrics.

* Enhance context management to maintain technical precision over multi-turn dialogues.

* Update the chatbot iteratively to address common misconceptions and optimize learning pathways.


## Data Analytics and Evaluation:

* Collect and analyze chat logs, user ratings, and completion metrics to evaluate prompt effectiveness.

* Identify patterns in response accuracy, clarity, and latency to determine top-performing techniques.

* Use statistical analysis to compare prompt families and inform selection of best practices.


# Results

Through systematic testing across various prompt engineering techniques—including zero-shot, few-shot, chain-of-thought, prompt template, and generative knowledge—generative knowledge-based prompting emerged as the most effective method for the Cybersecurity AI Study Companion.

While techniques like few-shot and prompt templates were often accurate and efficient, they typically lacked depth or failed to explain underlying cybersecurity concepts. Zero-shot and chain-of-thought approaches occasionally provided partial or incorrect results, particularly when deeper reasoning or context was needed.

In contrast, generative knowledge prompting consistently delivered the most accurate and pedagogically valuable responses. This approach not only identified correct answers, such as classifying Role-Based Access Control (RBAC) correctly and calculating password entropy, but also offered detailed explanations grounded in foundational knowledge. These responses were structured, informative, and aligned well with educational objectives.

Generative knowledge prompts effectively enhanced cybersecurity learning by:

* Breaking down complex topics like access control models and entropy calculations,

* Reinforcing conceptual understanding,

* Encouraging logical reasoning and problem-solving,

* Providing contextual examples and justifications.

These findings suggest that integrating generative knowledge-based prompting into AI-powered cybersecurity study companions can significantly improve learning outcomes. It promotes a deeper grasp of foundational concepts and offers a scalable, engaging tool for students and self-learners in cybersecurity.

The full set of evaluated prompts and results can be found here: [TEST_RESULTS.md](./TEST_RESULTS.md)

# Further research

* Explore reinforcement learning to auto-tune prompt parameters in real time.

* Integrate multimodal elements (diagrams, code snippets) into prompts for richer explanations.

* Extend to other technical domains (digital forensics, secure coding) to validate generalizability.

* Develop visualization dashboards to trace prompt→response workflows and optimize at scale.


