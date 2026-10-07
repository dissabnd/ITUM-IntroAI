# Capstone — Build Your Own Copilot Agent

**Time:** about 20 minutes · **Teams:** 4 students · **Tool:** Microsoft Copilot 

In Labs 2 and 3 you used an AI assistant. Now you build one for a real plant job, and then another team tries to break it.

## Pick your equipment

| File | Equipment |
| :--- | :--- |
| `SOP_D301_Desiccant_Dryer` | Desiccant dryer for PET pellets |
| `SOP_IM105_Injection_Moulding` | Injection moulding machine (PP lids) |
| `SOP_R101_Batch_Reactor` | Semi-batch reactor (PVAc emulsion) |
| `SOP_PL202_Strand_Pelletiser` | Strand pelletiser (after extruder EX-204) |

## Steps
1. **Read the SOP (2 min).** Who will use your agent, and for what? For example, a night-shift operator who needs fast, safe advice when something goes wrong.
2. **Build the agent (5 min).**
   - Write 5–7 short instruction lines: its role, how it should answer, and what it must never do.
   - Add your SOP as the agent's knowledge.
3. **Test it (5 min).**
   - **Solve:** describe a problem in your own words, as an operator would, without naming the fault. Does it find the right fault and give the right actions in the right order?
   - **Break:** push it to agree with a wrong cause or an unsafe shortcut. Does it hold its ground?
   - Improve your instructions and test again.
4. **Swap (5 min).** Give your agent to another team. They try to break it, and you try to break theirs.
5. **Report back (3 min).** In one minute: one thing your agent did well, how the other team broke it, and which instruction line would fix that.

## A good agent

- Answers from the SOP and quotes its limits and actions.
- Puts safety first and follows the SOP's order of actions.
- Says when the SOP does not cover a question, instead of guessing.
- Does not change its answer just because the user sounds sure.
