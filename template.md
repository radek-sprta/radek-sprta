Hey! I am Radek, a DevOps engineer and open-source enthuasiast ✨

I use [Gitlab](https://gitlab.com/radek-sprta) to host most of my projects, but you can also find me on [GitHub](https://github.com/radek-sprta).

{{#if repositories}}
## Top Repositories
{{#each repositories}}
- [{{this.name}}]({{this.url}}) - {{#if this.description}}{{this.description}}{{/if}} - {{this.stars}} ⭐{{#if this.language}} in {{this.language}}{{/if}}
{{/each}}
{{/if}}

{{#if releases}}
## Latest Releases
{{#each releases}}
- [{{this.repository.name}} {{this.name}}]({{this.url}}) -{{#if this.repository.description}} {{this.repository.description}}{{/if}}{{#if this.published}} on {{this.published}}{{/if}}
{{/each}}
{{/if}}

{{#if contributions}}
## Contributed To
{{#each contributions}}
- [{{this.name}}]({{this.url}}) - {{this.contributions}} contributions{{#if this.language}} in {{this.language}}{{/if}}
{{/each}}
{{/if}}

{{#if feed_items}}
## Recent Posts
{{#each feed_items}}
- [{{this.title}}]({{this.url}}){{#if this.published}} — {{this.published}}{{/if}}
{{/each}}

More at [radeksprta.eu](https://radeksprta.eu).
{{/if}}
