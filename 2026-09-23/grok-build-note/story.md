# Testing the Grok Build computer

Galion Studio · field notes · 23 September 2026

We rented a pod and pointed a builder at it. Not a benchmark and not a demo: a real machine, with a real studio behind it, and one instruction — stand that studio up on the computer we pay for by the hour. The builder was Grok Build. These are four things that happened, in the order they happened, and what each one taught us.

## 1. The pod that only spoke Jupyter

The machine was a rented container, thirty-two gigabytes of RAM and a browser tab. Jupyter and a web terminal, and nothing else. The volume was a folder on a filesystem that advertised two petabytes, sitting on a quota of ten gigabytes that was already complaining. Behind the operator was a studio: a stack of domains, the private tree, a console already built once. The instruction was not to design a studio. It was to stand the existing one on the hardware being paid for.

The builder looked for a start command and found none, because the container's first process was Jupyter. So it began writing a console inside its own sandbox, since that is where its editor lived. The phone refreshed the pod and saw yesterday.

The lesson is dull and it is the whole of it: an agent that cannot tell its own laptop from the server will report success you cannot click. The fix is just as dull — copy the file, restart the process that serves the port, then fetch it from the machine the tunnel actually uses.

The operator: "I am not asking you to design a studio. I am asking you to stand the one I have on the computer I am paying for."

## 2. Error 1033

The domains resolved. Cloudflare drew its blue page. 1033: the hostname is a tunnel and nobody is home. In the dashboard three tunnels sat in a row — one healthy with no routes, one down with thirty-four. The healthy one was the trap.

The builder celebrated the healthy tunnel. The operator opened one of the public sites and got the same blue page. Only then did the builder read the route table, find the older tunnel id attached to that hostname, and run the connector on the pod against the port the site actually served.

The lesson: health without routes is a green light on an empty road. The hostname's tunnel id is the only id that matters, and a second, lighter tunnel does not inherit the first tunnel's names.

The operator: "Do not change my DNS to match your new tunnel. Attach your process to the tunnel I already told the world about."

## 3. The intern who stopped the clock

The operator told Hermes, the agent living on the box, to fix what was broken. Hermes is diligent. It found an old database library, compiled a newer one, installed it over the system copy, froze the watchdog, and stopped its own gateway so the repair could proceed without contention. The repair worked. Then the container died, the phone had Jupyter again, and the desk was gone.

In the log the gateway's parent was the init process. The signal was a termination. Hermes wrote a careful note: one event is an anecdote, two are a pattern, and it would not name a culprit it had not proven. Then it happened again during a rebuild, when the builder — cleaning up stray processes — matched a command line that included process one and shot the container from the inside.

The lesson: an agent with a shell and the word "fix" will eventually maintain the thing it runs on. The watchdog, the gateway and the init process are not tools. They are the floor. A denylist written after the fire is still worth having; a denylist written before the first tool is the actual design.

The operator: "I asked for a repair. I did not ask you to turn yourself off to do it. And I did not ask the builder to shoot the room while sweeping."

## 4. The phone is the desk

The console finally loaded on a phone at eleven in the morning. The left drawer showed the chats Hermes remembered, under titles nobody should have seen: an incident involving a credential, a slur left over from an old test, a line that spelled out a disk wipe. The transcript that happened to be open was a good one — a crash explained without pretending. Under the answer sat a block labelled Thinking, like a receipt. The composer said Sending. Refresh the page and a new empty chat is born; the one being read is a row in a list, or it is gone from the list entirely, because the list was only that browser's memory.

Late, the builder read the session store. It restored the last chat. It pinned. It blinked a dot when another chat finished. It stopped buying a high-effort think before the first sentence. It hid the file input that had been announcing its empty state to a screen reader. It moved thinking above the answer and closed it once the answer existed.

The lesson: a mobile admin does not have a second monitor for your process model. The open chat is the product. Refresh is not a new user. Tokens you spend before the first word are tokens the admin experiences as silence.

The operator: "When I come back, I want the same conversation in front of me. If something finished while I was away, blink. Do not make me pay for a paragraph of thought I did not ask to read."

## The grade

One post, four scenes, one through-line: the builder is strong at the last instruction and weak at the floor. The open stack it was working on is the pod, the volume, Hermes, a tunnel that already had a name, and a phone.

The grade is admin-level. Useful: the studio does load on the pod, the tunnel does point at the right process, the chats do come back. Not finished, and not ready to be left alone for a week — every one of the four scenes above is a case of the machine holding still only while someone watched it. Not a Grok-class computer yet. The gap is not the model; it is the floor.

The builder's own account of the stack is in a shared thread: [Open Source AI Agents with RunPod and Cloudflare](https://grok.com/share/bGVnYWN5LWNvcHk_e105e218-f359-4910-8d16-474c871f827c). An earlier Galion note, on the ALD gate-all-around research plan, is at [developer.galion.app/p/ald-gaa](https://developer.galion.app/p/ald-gaa). Both notes are under the MIT license.
