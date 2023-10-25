# Documentation Repository

Welcome to our Documentation Repository! 🚀

## Overview

This repository serves as the central hub when we want to work together with our DevOps Professionals on Project Documentation. Clear and comprehensive documentation is crucial for understanding our deliverables, projects, and complex environments. It not only benefits us internally but also plays a vital role in ensuring our customers have a seamless experience and clear understanding of the environment.

Navigate to our documentation: [Home Page](index.md)

> [!IMPORTANT]
> Please read carefully the guidelines outlined in the [Getting Started](xref:gettingstarted)

## Why Documentation Matters

Documentation provides a shared understanding and knowledge base for our team and our customers. It serves as a reference point, enabling us to:

- **Improve Collaboration:** Working together with customers on documentation ensures we capture their unique perspectives and requirements, leading to better solutions.
- **Ensure Clarity:** Having a clear overview from the beginning helps us build a strong foundation, reducing confusion and misunderstandings.
- **Enhance Customer Experience:** Well-documented processes and products empower our customers, enabling them to use our solutions effectively.

## How to Contribute

We encourage all team members to actively contribute to our documentation efforts. 

> [!NOTE]
> Of course, it should be clear that we are doing this effort as part of our deliverables, and hence it should be clear this is categorized as **engineering work (billable)**.

Want to contribute? Check out [Contributing to the project documentation](xref:contributing)

 Here's how you can get involved:

1. **Collaborate with Customers:** Engage with our users to gather insights and feedback. Their input is invaluable in creating user-friendly documentation.

2. **Add and Update Content:** Contribute by adding new documentation or updating existing content. Whether it's a guide, tutorial, or FAQ, your contributions make a difference.

3. **Review and Improve:** Review existing documentation to identify areas of improvement. Even small edits can enhance clarity and usability.

## GitHub Actions and Hosting

We have set up GitHub Actions to automate the building process of our documentation artifacts. Through this automation, we can host a static website (e.g. on IIS) with the content of this repository. This ensures that our documentation is always up-to-date and easily accessible to both our team and users.

Our documentation artifacts are generated automatically through GitHub Actions. When making changes, simply commit your updates to the repository. GitHub Actions will take care of the rest, ensuring our static website is continuously updated. For now, there's no automatic deployment available, so we still need to manually copy the artifacts to a folder under IIS.

> [!NOTE]
> When hosting your website under IIS (used by DataMiner), you will still need to configure the default file (index.html) so you can browse easily to the folder (e.g. https://`hostname`/Documentation)

## Let's Build Something Great Together!

Thank you for contributing to our documentation efforts. By collaborating, adding new content, and maintaining the existing resources, we can create a knowledge base that benefits everyone. Together, let's build exceptional products, provide outstanding support, and deliver an exceptional experience to our customers.

Happy documenting! 📚✨
