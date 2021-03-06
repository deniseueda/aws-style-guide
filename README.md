# AWS Style Guide
One thing that bothers me when I go work in other job is the different way of organizing and naming capabilities of AWS services that each company has. To try to join ideas and, inspired by the [ruby style guide](https://github.com/bbatsov/ruby-style-guide), I decided to create a common sense of organization to AWS resources.

If you just started a AWS account now for your company then you can use this guide as a start line. If you have requirements that is unusual then you can fork this guide and keep updating to let people know how you solved your problems.

I do not know everything, but I hope the community can help me sharing their ideas in this repository.

## Elastic Cloud Computing

### Naming Instances

Naming instances is a important step to keep them organized. The name must to have a product prefix, a group prefix, an accountant and the region following by the company domain. Well, depending of the company, the group prefix can be optional. This is the pattern:

```
[product prefix].[group prefix (optional)].[accountant].[region].company.com
```
Some examples:

```
upd.cap.a.us-east-1.company.com
upd.b.us-east-1.company.com
group.workers.c.eu-west-1.company.com
```

### Tags
Tags are an important way to keep instances organized, and the essential tags for every instance is product and environment. Keeping instances well tagged, we can filter them in the cost explorer.

Some examples:
```
'Product' => 'my-product-slug',
'Environment' => 'production'
```

### Security groups
Every instance must to have two security groups by default and they are office and home-office. To add rules as needed.

## How to Contribute?

It's easy, just follow the [contribution guidelines](https://github.com/lucasosf/aws-style-guide/blob/master/CONTRIBUTING.md).

# License

![Creative Commons License](http://i.creativecommons.org/l/by/3.0/88x31.png)
This work is licensed under a [Creative Commons Attribution 3.0 Unported
License](http://creativecommons.org/licenses/by/3.0/deed.en_US)

# Spread the Word

A community-driven style guide is of little use to a community that doesn't know
about its existence. Tweet about the guide, share it with your friends and
colleagues. Every comment, suggestion or opinion we get makes the guide just a
little bit better. And we want to have the best possible guide, don't we?

Cheers,<br/>
[Contributors](https://github.com/Lucasosf/aws-style-guide/graphs/contributors)
