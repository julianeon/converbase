# About

An app and dashboard where you can answer your support questions, then use those answers to train an AI assistant which will eventually take over support for you.

The basic architecture is as follows.

On the front end, there's a React app with a dashboard where the admin sees user questions and answers them. Questions the admin selects can be marked for AI learning.

On the back end, there's a DB where all user questions are saved, along with a field to be included in the AI material learning set.

The AI part will be developed as a locally hosted LLM which is trained on these questions, then interfaces with the front through a 'bot' which forwards new questions as API requests to this local LLM.

Over time, as the admin selects more questions and the AI gets trained on them, its responses should get better and better, eventually taking over most of the work from the human admin.
