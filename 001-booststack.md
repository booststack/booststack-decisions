# Boost Stack will make launching new products easier and faster.

## Status
Draft

## Context

There are a lot of SaaS companies getting started. Most need very similar foundational pieces such as accounts, users, billing, authentication, etc. A common practice to get started quickly is to use tutorials that walk you through getting these functionality setup or including a library into your app (such as [devise](https://github.com/plataformatec/devise)). These practices have a number of problems.

### Time Spent On Undifferentiated Components
These pieces don't really help the company to differentiate their offerings but they do require dev time to build out and customize, even with a perfectly written tutorial together with a library such as devise. This investment in time is better spent on talking with customers and finding product market fit in the early days.

### Subpar Customer Experience
When using a tutorial and/or a library to build out these key foundational pieces, these pieces are usually subpar compared to existing companies because they aren't the most important areas to focus on initially. As a result, customers will get an experience that will likely be worse than what they are used to.

### Limited Scalability
These tutorials are usually intended to teach you and not be used in production so when you encounter some moderate success, you code does not scale up and requires a massive scramble to patch up the code, implement partitioning strategies or rewrite the breaking pieces.

### Unmaintained Future
When these pieces are written internally, the company is committing to not only write the code but also to maintain it. However, the reality of the situation for many is that these areas just become dormant parts of the code base with no maintenance work going into it because they aren't really improving the value delivered to customers.

There is an alternative approach that is possible.

## Decision

Boost Stack will be an opinionated way to build products. It will provide components and configuration strategies to make going from zero to real product fast and make it easy to use these components with minimal maintenance. 

This is possible due to a few reasons:

### Self-Contained Packages
Docker containers make it possible for these foundational pieces to be provided in a way that allows developers building products to use them without much of the maintenance overhead. A standardized set of interfaces will allow usage of these components without knowledge of the technologies that power these containers.

### Avoid Future Problems
When building a product, by making some sound decisions early on, you can avoid a lot of pain in the future.  Usually, these decisions don't make the most sense for a startup because they slow you down due because they aren't the right things to focus on.

## Consequences

By reducing the cost of entry for new products, I'm hoping that a lot more new businesses are attempted and as a result, many more problems are solved for people.