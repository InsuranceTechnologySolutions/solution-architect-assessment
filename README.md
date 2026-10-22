# Solution architect assessment 🛠️

Welcome! This assessment is about how you approach a real problem, explain your ideas and respond to a change in requirements. We’re interested in your thinking, not in one “right” answer.

**About the times:** These are the time allowed for each activity during the interview. They are not limits on how long you can prepare. Please keep your preparation simple and focused; we want to discuss your approach, so your artifacts / outcome does not need to be super polished. 

## Part 1: The case ⚓

Imagine we’re building a **Know Your Customer (KYC)** system for marine insurance. Before an insurer agrees to insure anything, it assesses the risk. Vessels can be valuable, and it may be hard to see who owns or controls them. We want to identify parties (such as owners) and vessels that may be high risk, and understand how they are connected.

Design a system that brings useful information together and makes the risk clear. Focus on sanctions against the vessel and its Ultimate Beneficial Owner (UBO). The vessel’s flag and the country where the UBO is based also matter. Sanctions may mean the insurer cannot provide cover, depending on the rules that apply. State your assumptions; we’ll discuss them.

The tool is advisory. It should show risks, possible sanctions restrictions and the information behind them, the underwriter uses this information to decide what to do next.

Look into terms such as **Flag**, **Owner**, **UBO**, **AML**, **FATF** and **OFAC** as part of your preparation. Be ready to discuss what they mean and how they relate to your solution.

For background, see [MarineTraffic’s Risk & Compliance Methodology](https://support.marinetraffic.com/en/articles/11172276-risk-compliance-methodology). You do not need to copy their approach.

As a starting point, you could suggest that risk gets lower the further a party is from a person or company with an identified risk in the ownership chain. For example, a party one link away might have less risk than the party with an identified risk, and a party two or three links away might have less again. This is only an idea to discuss, not a required or legally approved rule. Keep this general risk score separate from sanctions rules: sanctions may still prevent cover even when the sanctioned owner is several links away. Show a risk label and explain what it is based on, so an underwriter can make a decision.

Assume the system will use existing data sources. Think about what information it needs, how reliable and up to date that information is, and how regulations could affect the result. For example, there may be rules against doing business with parties in certain countries. State your assumptions.

**Prepare two 15-minute presentations of your solution, one for each audience:**

- **Product owner or non-technical manager:** Explain what you would build and why it matters. Talk about likely costs, risks, progress and how you would keep people informed. Rough estimates are fine; explain your assumptions.
- **Technical team:** Explain how you would build it. Diagrams are welcome 🙏. Be ready to discuss your design choices.

## Part 2: Coding assessment ⌨️ (20 minutes)

**Problem:** Build a simple KYC app for marine insurance, based on Part 1. A user should be able to search for a vessel, person or company and see its risk profile, including the reasons for the risk and any related people, companies or vessels and their risk profiles.

Keep it simple: a search box and results are enough. You do not need data-entry forms or a polished user interface. Use sample data to show your model, no external source. You can create the data yourself or use a library such as Bogus or AutoBogus. You do not need to connect to real data sources.

There is no time limit for preparation. The 20 minutes is for showing and discussing your work during the interview. You may use an LLM and any programming language or tools you like. The app does not need to be perfect or ready for real use.

**The main focus is the design and model behind your app:** how they reflect your Part 1 proposal. Be ready to explain the main concepts, how they relate to each other, and your DTOs and APIs. We’re interested in why you made those choices, not how much code you (or the 🤖) wrote.

## Part 3: The curveball ⚾ (15 minutes)

The requirements will change. We’ll explain what has changed during the interview and discuss it together, using a whiteboard if helpful. We want to see how you adapt, consider options and explain your thinking—not how quickly you find an answer.


**Additional notes:** Use any tool you like for your presentations, such as PowerPoint, Google Slides or GitHub Pages.

For the coding part, please send your repository link to stig.nielsen@instech.no before the interview. He will share it with the team.

If you have questions, please get in touch.

Good luck! 🙂
