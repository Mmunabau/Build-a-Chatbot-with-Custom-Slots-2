<h1>Build a Chatbot with Amazon lex</h1>

<h2>Description</h2>
 Amazon Lex is a fully managed service by AWS for building conversational interfaces into applications using voice and text. It uses automatic speech recognition (ASR) to convert speech to text and natural language understanding (NLU)
<br />

<h2>  How I used Amazon Lex in this project </h2>
 we used Amazon lex to creat a responsive Banking chatbot that respond to customers accounts request my creating a custom slot type.
<h2>Skills Demostrated:</h2>

- <b>Cloud Computing Proficiency: Configuring AWS services like IAM, Lambda, and Amazon Lex to build and manage conversational interfaces</b> 
- <b>Natural Language Understanding (NLU): Designing intents, utterances, and slot types to enable the chatbot to comprehend and respond effectively to user queries.</b>
- <b>Problem-Solving with Lambda: Developing and deploying AWS Lambda functions for custom business logic and advanced intent fulfillment..</b>

<h2>Utilities used</h2>
<ul>
  <li>AWS console</li>
   <li>Amazon Lex</li>
</ul>
<h2>Program walk-through:</h2>

<p align="center">
 Slots: Slots are pieces of information that a chatbot needs to complete a user's request By adding custom slots in utterances, my chatbot's user experience is  enhanced- the bot will automatically register which account type the user is trying to check, and will [explain how this saves the bot from asking for the account ] I created a custom slot type to represent the different account types that a banking customers could have.A customers slot type was required as the default slot types did not accommodate for account type (e.g
 Checking,Savings & Credit:) <br/>
 <img src="images/lx1.png" height="80%" width="80%" alt="key steps"/>
<br />
 
<br />
  Connecting slots with intents:This slot type has restricted slot values, which means' the chatbot will only respond to the slot type provided. we made sure that our BankerBot only recognizes and accepts the bank account types we offer. I associated my custom slot with CheckBalance, which is a new intent i created that helps my bank's customers check its users account balances.
  <br/>
<img src="images/lx2.png" height="80%" width="80%" alt="key steps"/>
<br />

<br />
 Slot values in utterances: I included slot values in some of the utterances (i.e. user inputs) by... For example'.I defined the utterance "Whatʼs the balance in my {accountType} account?".This is an example of an utterance that expects the slot account
 Type.<br/>
<img src="images/lx3.png" height="80%" width="80%" alt="key steps"/>
<br />
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
