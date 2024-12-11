Leaves

Terms:
Theorem - A proven theorem. Onchain this is represented by a zk proof of a correctly formed lean type inference over the statement.
Closed-source Theorem. A proven Theorem without it's associated open source proof.
Conjecture - An unproven theorem with a possible bounty. Conjectures become Theorems. A conjecture consists of a list of axioms and a logical expression intended to hold under the axioms.
Dependency - Conjecture or Theorem used in an Attempt.
Attempts - attempts at Theorems. Attempts can refer to any number of other Conjectures and Theorems
Models -

Relationships:
A conjecture used in an attempt is called a dependency
A conjecture used in an attempt is a valid dependency iff the set of axioms in the conjecture is a subset of the attempt's theorem.
A conjecture becomes a theorem if a zk proof of a lean type system exists.
A proven theorem pays the reward for all rewarded conjectures and the remainder
to the proover
The prover must be the creator of the attempt.
Only the owner of an attempt can update the attempt.

Extra rules:
Only one attempt can be registered for a theorem per week. This is a rate limit
to avoid 'proof MEV'. Though this can lead to 'attempt starvation' where an entity DOSes attempt creation by monopolising top of block attempt creation.

Modified conjecture problem: Anyone can construct a new attempt including all previous in-attempt proven conjectures and reneg on the rewards for the sub conjectures.
Make an entity that reserves the right to block attempts from being rewarded?

We will need some access control over Attempts. - the originator likely

Tooling required:
Attempt uploader / updator
Lean package manager s.t. theorems are pulled from the structure.

Conjectures can have permissionless rewards attached to them.


The construction of an attempt can fix any subset of its rewards onto a conjecture used in the attempt.

Once an attempt has assigned reward to an attempt it cannot undo so. Unless it is a kyc pool managed by Nethermind :P

Total Value of a Conjecture. Easier to measure the lower bound -> an attempt 

Axiom adition: how often is it that there is a missing axiom?


Games, MEV etc

All proofs can be frontrun....

Timing games, stealing proofs etc

High burn on theorem and conjecture creation? Use potential rewards to loan out the creation value - doesn't work. Hmm.

Rate limits on actions

Keeping parts of the proof private?

Perhaps we don't reveal the structure of the proofs at all, i.e. keep the related conjectures private so that
each conjecture simply has a value. This leaks little about the current state of proving a conjecture while keeping
some amount of fairness.


Financial rewards may actually not make sense. There is good reason for scientists to reject payment for the creation of open knowledge.

Is there a fundamental problem to crypto. Does the lack of privacy preclude social games?

What kind of games are there?


Open completioni games. They are the same class as unathenticated exploits.
Encrypted mempool may be the only solution.

Open math problems for good:

All meaningful proofs should be colllated in one place. It should no longer be the case that meaningful proofs have to
be studied in their minutia to be convinced of their correctness. This is the goal of machine checkable proofs and the goal of communities
like the xena project for Lean. We propose to go further, let's have a global, immutable record of all results proven to be correct.
Not in a repository which may not be coorect.
Use this to onboard universities and mathematicians onchain.
Inclusion into this repository is impossible without concrete proof that the solution is correct. Not even the maintainers of the repository can
include a statement without the correctness demonstrated.


Commercialisation:
The MEV problem leads to the following conclusion:
All problems are stated open-source. Anyone is welcome to solve them.
Only those registered on our platform with us can be rewarded for the solution?
With control over the incentivised solver set Nethermind can block any solver who exhibits malicious behaviour.

ZK lock-in - FUCK YESSSSSS, you prove you have the solution without revealing the proof.
Basically an encrypted mempool. This resolves front running proof submission.
The submitter of the zk proof is partially rewarded and the Conjecture becomes a 'closed source' theorem. 
The submitter recieves the remainder of the reward if they submit the Lean proof in its entirity.
Any submitter can transition a closed source theorem to an open source theorem after a claim window.
tragidy: It is the case that no rational blockbuilder should accept a zklockin. However, I defer to 1 of N security
and assume one builder / proposer wishes this protocol to execute unimpeeded.

This still doesn't solve the 'conjecture extension' issue.


Do we rely on a reputation system to solve the bullshit conjecture problem?
Proving theorem equivalance is impossible in the general case - halting problem I believe.





ZK proofs of exploitation!!!!!!!! A new product!!!! Awesome!!


Idea:
Every protocol has a locking mechanism. Anyone can trigger the locking mechanism
if they submit a zk proof of onchain execution which results in a violation of the protocols formal model.
In submitting this proof the would be exploiter is fairly and automatically rewarded.

