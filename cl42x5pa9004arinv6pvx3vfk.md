## GitLab introducing Free tier user limit

[Sid Sijbrandij](https://about.gitlab.com/company/team/#sytses), Co-founder and CEO of [GitLab](https://about.gitlab.com/), announced, in a [blog post](https://about.gitlab.com/blog/2022/03/24/efficient-free-tier/), that beginning June 22, **the Free tier of GitLab SaaS will be limited to 5 users** per [namespace](https://docs.gitlab.com/ee/user/group/index.html#namespaces).

> These changes allow us to invest more in research and development for product innovation of the GitLab DevOps Platform.

The motive included in the statement is extremely vague, and GitLab states that this will "impact fewer than 2% of Free tiers users within 0.3% of the namespaces". The issue with throwing out a number without additional context, is that it can be perceived negatively, no matter how you spin it. If the number is large, then GitLab is pulling a "bait and switch" tactic for many of its customers. If the number is small, then GitLab has better ways to increase profit without scrounging for money from Free users.

[Transparency is one of GitLab's values](https://about.gitlab.com/handbook/values/#transparency), and typically, I would be commending them for it. For example, let us compare when GitLab made a similar change by [limiting CI/CD minutes for Free tier users on GitLab.com](https://about.gitlab.com/blog/2020/09/01/ci-minutes-update-free-users/) in late 2020 which affected a similar number of users.

> While we are excited by this exponential growth, our underlying costs to support this growth have increased significantly.

Sid Sijbrandij stated the motive for limiting CI/CD minutes for the Free tier more directly, and the underlying costs of running compute for CI/CD pipelines is more obvious. The alternatives of paying for minutes or running self-hosted runners was not unfeasible. However, in the case of limiting the amount of free users per group, the operational costs of supporting each GitLab user is unclear.

So due to the lack of transparency, I am left here hypothesizing potential reasons why GitLab would make this move. Are the costs of running GitLab.com getting out of hand? Is GitLab having issues scaling GitLab.com, and now they are trying to push organizations to self-hosted instances? [Insert preferred higher power here] forbid this change and lack of transparency is a byproduct of [GitLab going public](https://about.gitlab.com/blog/2021/10/14/gitlab-inc-takes-the-devops-platform-public/). Whether GitLab is trying to prevent the system from being abused by a few bad actors, or if they are trying to extract as much cash as possible out of its users, more clarity on the motive would be helpful.

![GitHub](https://about.gitlab.com/images/blogimages/github-news-cover.png)

And then there is GitHub. Years ago, GitHub was the popular and default choice and GitLab was the underdog power play. GitHub was an SCM with a couple of simple merge request extensions, and GitLab provided tools for the entire software development lifecycle. GitHub was closed-source and required a paid plan for any private organizations, while GitLab was open and free. The feature gap GitLab provided is what allowed its "exponential growth", but GitHub has closed that gap significantly in the past couple of years. To top it off, **GitHub does not limit free users in an organization**.

So what are the options? Ideally, GitLab would have an entry-level paid model, but [GitLab removed the Bronze/Starter tier](https://about.gitlab.com/blog/2021/01/26/new-gitlab-product-subscription-model/) in early 2021, which would have given Free tier organizations impacted by this change a $60/user/year upgrade path. Now, the lowest paid tier is Premium at $228/user/year, which can be a steep cost to pay for a small group. Besides upgrading to Premium, the only other option is to self-host your own GitLab instance, which can be daunting, especially if you want to build a high available and scalable instance.