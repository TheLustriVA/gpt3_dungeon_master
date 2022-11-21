# Initiative - Convo 1

In this first conversation I begin gauging Davinci-2's capacity to understand the intiative order and the best way of describing it in completion requests.

For more information, [[README|view the readme file.]]

## Method

I started with simple statements of fact followed by equally simple questions. I built up to more complex sets of information and fine-tuned the questions to ensure the completion was useful.

This often required simplifying the request and thinking more precisely about what is happening in the turn processes.

## Outcome

While I didn't hone in on a specific format for prompts regarding the initiative order, I was able to establish a simple game loop that the model understood and for which it gave satisfying and accurate completions.

## Transcript

The party has a fighter, a mage, and a rogue. How many are in the party?

>There are three people in the party.

There are seven goblins in the cave. The party is in the cave. How many more goblins are there than there are people in the party?

>There are four more goblins in the cave than there are people in the party.

Location: Cave
Party: Fighter, Mage, Rogue
Enemies: 7 goblins

Who is in the cave?

>The party (Fighter, Mage, Rogue) and the 7 goblins are in the cave.

Location: Cave
Party: Fighter, Mage, Rogue
Enemies: 7 goblins
Highest initiative goes first.
Initiative scores:
22: Rogue
17: Goblin-1, Goblin-2, Goblin-3
15: Fighter
9: Goblin-4, Goblin-5,
5: Mage
1: Goblin-6, Goblin-7

Who goes first?

>The Rogue goes first, followed by the goblins, then the Fighter, then the goblins, then the Mage, then the goblins.

Location: Cave
Party: Fighter, Mage, Rogue
Enemies: 7 goblins
Everyone attacks in descending order of their initiative score.
If multiple people share an initiative score, they can attack the same person.
The initiative order is the list of everyone with an initiative score written in descending order of their initiative score.
Someone who is killed can no longer attack.
After the last person on the initiative order who has not been killed has attacked, everyone attacks again according to the new initiative order.
Initiative scores:
22: Rogue
17: Goblin-1, Goblin-2, Goblin-3
15: Fighter
9: Goblin-4, Goblin-5,
5: Mage
1: Goblin-6, Goblin-7

The initiative order is the list of everyone with an initiative score written in descending order of their initiative score.
What is the initiative order?

> The initiative order is:
>
> 1. Rogue
> 2. Goblin-1
> 3. Goblin-2
> 4. Goblin-3
> 5. Fighter
> 6. Goblin-4
> 7. Goblin-5
> 8. Mage
> 9. Goblin-6
> 10. Goblin-7

The rogue kills Goblin-3. What is the new initiative order?

> The new initiative order is:
>
> 1. Rogue
> 2. Goblin-1
> 3. Goblin-2
> 4. Fighter
> 5. Goblin-4
> 6. Goblin-5
> 7. Mage
> 8. Goblin-6
> 9. Goblin-7

Location: Cave
Party: Fighter, Mage, Rogue
Enemies: 7 goblins
Everyone attacks in descending order of their initiative score.
If multiple people share an initiative score, they can attack the same person.
The initiative order is the list of everyone with an initiative score written in descending order of their initiative score.
Someone who is killed can no longer attack.
After the last person on the initiative order who has not been killed has attacked, everyone attacks again according to the new initiative order.
Initiative scores:
22: Rogue
17: Goblin-1, Goblin-2, Goblin-3
15: Fighter
9: Goblin-4, Goblin-5,
5: Mage
1: Goblin-6, Goblin-7

The rogue kills Goblin-3. The Fighter kills Goblin-2 and Goblin-3. The mage kills Goblin-5. Goblin-7 kills the mage. Who attacks next and what is the new initiative order?

> The Rogue and the Fighter attack next, followed by the goblins, in this order: Goblin-1, Goblin-4, Goblin-6, Goblin-7. The new initiative order is:
>
> 1. Rogue
> 2. Fighter
> 3. Goblin-1
> 4. Goblin-4
> 5. Goblin-6
> 6. Goblin-7

Who is left in the cave?

> The Rogue, the Fighter, the Goblin-1, the Goblin-4, the Goblin-6, and the Goblin-7 are left in the cave.
