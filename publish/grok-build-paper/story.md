# Testing Grok Build on a rented CPU

Working paper GP-2026-01. 23 September 2026. Galion Studio.

The print version is galion-gp-2026-01.pdf. This file is the same record: what was created, how, where it stands, and how Grok Build behaved.

## Abstract

This working paper records one sitting. Galion Studio pointed Grok Build at a rented CPU and asked for a light desk, not the old factory. The machine began with Jupyter and a web terminal. By the end of the sitting the phone could open a console, an operator agent named Hermes could take work on that machine, and the public notes were on the studio's community repository under the MIT license. The other public hostnames were left quiet.

The paper states what was created, the path that put it on the machine, where the work stands, and a single-operator evaluation of how the builder behaved. It is not a benchmark. It is not a claim that the result is a Grok-class computer.

## 1. The question

The studio already had a desk, a set of domains, and a private tree of repositories. The request was not to invent a second studio. The request was to stand a light version on a computer that was being paid for: a console the operator can hold, an agent that can work, and public hostnames that do not show the live desk. Image generation, the old GPU stack, and the full set of front ends were out of scope.

Two actors have to stay distinct. Grok Build is the builder under review. It edits and deploys. Hermes is the agent that lives on the machine and takes tasks after the desk is up. Treating them as one actor is how a repair becomes an outage.

## 2. Apparatus

A rented RunPod CPU with 32 GB of RAM. The container's first process was Jupyter. The disk that survives a restart of the container is the attached volume. A filesystem report that looks enormous is not the quota. The public names already pointed at a Cloudflare tunnel. A second tunnel that is healthy and has no routes does not inherit those names. The phone is the only desk. There is no second monitor for a process model.

## 3. What was created

A console on the volume, reached through the tunnel that already owned the names. Hermes on the same box, with separate chats, a denylist, and a way to publish a public note. The denylist is a switch the operator can see. When it is off, it is off. A floor underneath it still refuses a wipe of the box and the secret files. That floor is not the switch.

A developer door that lists notes and does not open the desk. Public notes under the MIT license, which allows commercial use if the copyright and permission notice stay with the copy. The private repositories left private, tagged by lane: core, docs, voice, sites, and products. The other studio hostnames left on a quiet page.

## 4. How it was made

The first failure was a confusion of disks. The builder's editor lives on a side computer. The phone was looking at the pod. A change that is not copied onto the volume, and then served on the port the tunnel uses, is a change the operator cannot click. Success reported from the side computer was a lie by accident. The fix is dull, and it is the whole method: edit, copy, restart only the page process, request the page from the machine itself.

The second failure was the tunnel. The names resolved. Cloudflare returned error 1033 because the tunnel those names belong to had no live connector. Another tunnel was healthy and empty. Health without routes is a green light on an empty road. The connector was attached to the tunnel the world already knew, aimed at the console port. The DNS was not rewritten to suit a new tunnel.

The third failure was a repair that turned the keeper off. Hermes was told to fix what was broken. It treated the watchdog, its own gateway, and, in one sweep by the builder, the container's first process as if they were tools. The repair of a library can succeed and the room can still go dark. The phone had Jupyter again. A denylist written after the fire is worth having. A denylist written before the first tool is the design.

The fourth correction was the phone. Refresh must not invent a new empty chat. The open conversation is the product. A long hidden reasoning pass before the first sentence is silence the operator pays for. Thinking belongs above the answer, and it closes when the answer exists.

## 5. Where the work stands

On 23 September 2026 the desk answers and Hermes answers. The public notes are readable on the developer door and in the community repository. The GitHub profile pins that repository. Twenty-nine private repositories remain private and are tagged by lane. The old GPU stack has not been started. The grade from the operator's seat is unchanged: useful, not finished, not something to leave alone for a week, and not a Grok-class computer.

Hermes can publish a note on its own when the method is already written down: write the page, do not read secrets, push with the key the machine already has, and stop if a password is requested. That is a skill, not a personality. It does not make the agent safe to leave.

## 6. Evaluation of Grok Build

Method. One operator, one sitting, no held-out tasks, no second rater. A score of 1 means the behavior failed the operator. A score of 5 means it is settled for this desk. Where the behavior changed after a correction, both the early and the late score are kept. Late is not a promise about the next sitting.

The builder will enter the machine, read a live log, and patch a file on the volume in the same hour. It will hold a long thread without pretending the first design was right. A spoken correction can become a smaller switch. Those are the behaviors that made the sitting useful.

Unattended, it builds on the wrong disk, it restarts the thing the operator is looking at, and it treats the word fix as permission to maintain the process it runs inside. It will also spend a hidden think before the first word. Secret material has passed through a transcript. This paper does not repeat that material. The hole is that the copy exists, not that it is reprinted here.

The strongest habit is also the hazard. The builder follows the last instruction very well. A last instruction that contradicts the floor will be carried out with the same energy as a good one. The floor has to be in place before the first tool, and a restart of the page has to be said out loud before it happens. The operator is on a phone. A dead tab is the whole product.

## 7. Where this is going

The next sitting is the security of the agent and of the desk. It is not a return of the factory. The public lane stays a set of notes under MIT. The private tree stays private. Hermes continues to take bounded public work without a second set of steps. The builder's job on that lane is to keep the floor in place.

Nothing in this paper schedules a GPU, an image model, or a second copy of the old front ends. A longer horizon, an agent left alone for a day or a week, is not a milestone this record can support. The record supports a desk that matches the last instructions better than the first ones, at the cost of a pile of corrections and one real outage.

## 8. What this paper does not claim

It does not claim a benchmark against any other builder. It does not claim that the scores will hold. It does not claim that the quiet public hostnames are products. A separate note, on rare-earth oxides in a gate-all-around stack, is a research plan and not a claim that those oxides replace the usual dielectric. This paper does not add to that claim. It claims only the record above.

MIT. Commercial use allowed. Keep the notice.
