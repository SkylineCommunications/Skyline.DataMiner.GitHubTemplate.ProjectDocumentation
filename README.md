# Documentation Repository

Welcome to our Documentation Repository! 🚀

## Overview

This repository serves as the central hub when we want to work together with our DevOps Professionals on Project Documentation. Clear and comprehensive documentation is crucial for understanding our deliverables, projects, and complex environments. It not only benefits us internally but also plays a vital role in ensuring our customers have a seamless experience and clear understanding of the environment.

Navigate to our documentation: [Home Page](index.md)

> [!IMPORTANT]
> Please read carefully the guidelines outlined in the [Getting Started](xref:gettingStarted)

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

## How to get started

> [!IMPORTANT]
> For Skyline employees: Please include a link from [InternalDocs - ProjectDocs](https://internaldocs.skyline.be/Projects/Projects.html) to this repository

1. Follow the steps described at [Creating a repository from a template](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template#creating-a-repository-from-a-template)
1. While creating the new repository, take into account the [GitHub Repository Guidelines](https://docs.dataminer.services/develop/CICD/Skyline%20Communications/Github/Use_Github_Guidelines.html) described in the DataMiner Docs. 
    1. Suggested Naming Convention: {customerAcronym}-DOC-NameOfProject
    2. Add/Change the license according to what is agreed with the customer
    3. Add GitHub repository topics: dataminer-doc
1. Once the repository is cloned, add your custom documentation available in the 'articles' folder. Suggest structure:
    1. overview.md: the purpose of the environment is documented with a high-level overview of the most important components
    2. features.md: key components of the environment, typically with subfolders
    3. infrastructure.md: user-oriented POV explanation of how the environment is built (architecture, database types, failover, etc.)
1. You can build a test build by following [Contributing to the project documentation](xref:contributing).
1. When you are happy with your changes, push them to the GitHub repository.
1. GitHub actions will make an artifact available that you put on your DataMiner which will host this as a static website. If you are interested, follow the steps in the section below.

### Tips

1. Change this README, and add a link to your front page so it is easily accessible through GitHub as well.
1. Add image files to the *images* folder if the file is referencing an image.
1. Consider using Mermaid for creating diagrams, etc. When creating images using Mermaid, take into account the dark and light themes. Make sure the images are readable in both themes.
1. Do not create lengthy pages. It is preferred to create smaller pages as the search is performed on page level.

## GitHub Actions and Hosting

We have set up GitHub Actions to automate the building process of our documentation artifacts. Through this automation, we can host a static website (e.g. on IIS) with the content of this repository. This ensures that our documentation is always up-to-date and easily accessible to both our team and users.

Our documentation artifacts are generated automatically through GitHub Actions. When making changes, simply commit your updates to the repository. GitHub Actions will take care of the rest, ensuring our static website is continuously updated. For now, there's no automatic deployment available, so we still need to manually copy the artifacts to a folder under IIS.

1. On your GitHub repository, go to the tab 'Actions'
1. Download the 'Documentation.zip'
1. Extract the archive in your DataMiner in the location 'C:\Skyline DataMiner\Webpages\Documentation'. Note the 'Documentation' folder is not available by default and can be created.
1. Configure the default file in ISS
    1. Go to Internet Information Services (IIS) Manager
    1. Find the 'Documentation' folder you have added
    1. In the 'IIS' section, double click on 'Default Document'
    1. Include the index.html on the list.
1. Navigate to 'https://`hostname`/Documentation' to view the website

## Let's Build Something Great Together!

Thank you for contributing to our documentation efforts. By collaborating, adding new content, and maintaining the existing resources, we can create a knowledge base that benefits everyone. Together, let's build exceptional products, provide outstanding support, and deliver an exceptional experience to our customers.

Happy documenting! 📚✨
