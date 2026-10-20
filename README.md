# Solution architect assessment 🛠️

Welcome! This is your chance to talk through a real-world problem, show how you approach a small proof of concept, and have some fun exploring a curveball. We’re way more interested in how you think and communicate than in a single “right” answer.

## Part 1: The case ⚓

For this case, imagine we’re building a **Know Your Customer (KYC)** system for marine insurance underwriting. Underwriting is often our first interaction with a customer, and vessels are high-value assets whose ownership and connections can be difficult to see. We want to identify potentially high-risk parties and vessels, and understand how vessel ownership connects them.

The assessment is about designing a system that brings relevant information together and makes risk understandable—not about finding one “correct” risk formula. Consider signals such as sanctions, politically exposed person (PEP) status, fraud, and opaque ownership. A PEP flag should inform an assessment, not automatically rule out a customer; sanctions may be disqualifying, depending on the applicable rules.

As a starting point, you could propose a simple rule for how risk is reflected across ownership relationships: the directly flagged party carries the highest risk, parties one ownership link away carry less, and risk decreases further with each link. For example, links at two or three steps away might receive progressively lower risk. Treat this as a business-rule assumption to discuss, not a prescribed or legally validated model. The system should show a risk tag and its basis so a human underwriter can decide whether to proceed.

Assume the system will use existing data sources. Consider what information you would need, how you would assess its reliability and freshness, and how relevant regulations could affect the result—for example, a restriction on doing business with parties based in a particular country.

You’ll present your solution to two audiences:

- **Product owner or non-technical manager:** What are we doing, why does it matter, and what might it cost? Talk through risks, progress, and how you’d keep stakeholders informed.
- **Technical team:** Walk us through the architecture. Diagrams are very welcome 🙏. We can discuss security, integrations and contracts, and the decisions and trade-offs behind your design.

## Part 2: Coding assessment ⌨️

We’ll identify a problem from the case for you to explore by creating a proof of concept (PoC). **NOTE: INSERT PROBLEM HERE**. Focus on demonstrating your approach and explaining your choices; the PoC doesn’t need to be production-ready.

## Part 3: The curveball ⚾

Something changes in the requirements. We’ll share the details during the interview, then work through the conundrum together using a pen, a whiteboard, and conversation. We’re interested in how you adapt, explore options, and communicate—not how quickly you arrive at an answer.


**Additional notes:** You can use whatever tool you want to present (PPT, Google presentaions, github pages), no constraints. 

When it comes to the coding part, please share the respository link up front. Send it to stig.nielsen@instech.no, and he will distribute it within the team. 

If you have any additional questions, please reach out.

Good luck! 🙂
