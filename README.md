Node-RED Watson Nodes for IBM Cloud
=====================================

[![Codacy Badge](https://api.codacy.com/project/badge/Grade/4f98536040924add9da4ca1deecb72b4)](https://www.codacy.com/app/BetaWorks-NodeRED-Watson/node-red-node-watson?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=watson-developer-cloud/node-red-node-watson&amp;utm_campaign=Badge_Grade)
[![npm-version](https://img.shields.io/npm/v/node-red-node-watson.svg)](https://www.npmjs.com/package/node-red-node-watson)
[![npm-downloads](https://img.shields.io/npm/dm/node-red-node-watson.svg)](https://www.npmjs.com/package/node-red-node-watson)

<a href="https://cla-assistant.io/watson-developer-cloud/node-red-node-watson"><img src="https://cla-assistant.io/readme/badge/watson-developer-cloud/node-red-node-watson" alt="CLA assistant" /></a>

### New in version 0.9.0
- Node-RED & IBM-Watson & Use of promises on API invocation & IAM URL construct migration & Removal of default endpoint of
    - Assistant V1
    - Assistant V2
- All Nodes now require Node-RED 1.0.x or above
- Remove watson-developer-cloud dependancy
- Remove code for redundant nodes

### New in version 0.8.2
- Node-RED & IBM-Watson & Use of promises on API invocation & IAM URL construct migration & Removal of default endpoint of
    - Document Translator node
    - Discovery node
    - Discovery Document Loader node
    - Discovery Query Builder node
    - Assistant V1 Workspace Manager node
- List Expansion list, and List Training data modes added to Discovery node
- Fix to Create Classifier mode in NLC node

### New in version 0.8.1
- Node-RED & IBM-Watson & Use of promises on API invocation & IAM URL construct migration & Removal of default endpoint of
    - Speech to Text node
    - Speech to Text Corpus Builder node
    - Natural Language Understanding node
    - Natural Language Classifier node
    - Language Identifier node
    - Language Translator node
    - Translator Util node
- New NLU Model Manager node.
- NLC CreateClassifier is broken until defect on ibm-watson is fixed.
- Remove X-Watson-Technology-Preview Neural translation option for Language Translator node
- Remove monolingual corpus option from Language Translator mode
- Added new modes to Language Translator mode
  - List Custom models
  - List Default models

### New in version 0.8.0
- In the 0.8.x releases the nodes are migrated to a node-red 1.0.x input
event callback function signature.
and migrated off watson-developer-cloud to ibm-watson as a npm dependancy.
Migrated nodes will not be compatible with pre 1.0.0 versions of node-red.
During the migration there will be a dependancy on both modules.
- Bump dependancy on node to >=10.0.0
- Bump dependancy on cfenv, request, file-type
- Bump dependancy on ibm-cloud-sdk-core to 0.3.7 (need to stay on 0.x, for STT Streaming to work)
- Node-RED & IBM-Watson & Use of promises on API invocation & IAM URL construct migration & Removal of default endpoint of
    - Tone Analyzer node.
    - Personality Insights node.
    - Visual Recognition V3 node
    - Text to Speech node
    - Text to Speech Corpus Builder node
- New Visual Recognition V4 node.
- Drop faces detect option from Visual Recognition V3 node.
- Fix to URL parsing for bound services.
- STT token manager no longer in ibm-cloud-sdk-core
- Update language lists for STT, TTS, Language Translator and Document Translator Nodes

### Watson Nodes for Node-RED
A collection of nodes to interact with the IBM Watson services in [IBM Cloud](http://cloud.ibm.com).

# Nodes

- Assistant (formerly Conversation)
    - Add conversational capabilities into applications.
- Discovery
    - List environments created for the Discovery service
- Language Identification
    - Detects the language used in text
- Language Translator
    - Translates text from one language to another    
- Natural Language Classifier
    - Uses machine learning algorithms to return the top matching predefined classes for short text inputs.
- Natural Language Understanding
    - Analyze text to extract meta-data from content such as concepts, entities, keywords ...
- Personality Insights
    - Use linguistic analytics to infer cognitive and social characteristics from text
- Retrieve and Rank
    - Creates a trainable search engine for your data  
- Speech To Text
    - Convert audio containing speech to text
- Text To Speech
    - Convert text to audio speech
- Tone Analyzer
    - Discover, understand, and revise the language tones in text.
- Visual Recognition
    - Analyze visual appearance of images to understand their contents

### Usage
Example usage flows can be found here [node-red-labs](https://github.com/watson-developer-cloud/node-red-labs)

### Contributing

For simple typos and fixes please just raise an issue pointing out our mistakes.
If you need to raise a pull request please read our [contribution guidelines](https://github.com/watson-developer-cloud/node-red-node-watson/blob/master/CONTRIBUTING.md)
before doing so.

### Copyright and license

Copyright 2018 IBM Corp. under [the Apache 2.0 license](LICENSE).
