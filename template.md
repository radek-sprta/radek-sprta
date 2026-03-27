Hey! I am Radek, a DevOps engineer and open-source enthuasiast ✨

I use [Gitlab](https://gitlab.com/radek-sprta) to host most of my projects, but you can also find me on [GitHub](https://github.com/radek-sprta).

{{#if repositories}}
## Top Repositories
{{#each repositories}}
- [{{this.name}}]({{this.url}}) - {{#if this.description}}{{this.description}}{{/if}} - {{this.stars}} ⭐ in {{#if this.language}}{{this.language}}{{else}}—{{/if}}
{{/each}}
{{/if}}

{{#if releases}}
## Latest Releases
{{#each releases}}
- [{{this.repository}} {{this.name}}]({{this.url}}) 
{{/each}}
{{/if}}

{{#if rss_items}}
## Recent Posts
{{#each rss_items}}
- [{{this.title}}]({{this.url}}){{#if this.published}} — {{this.published}}{{/if}}
{{/each}}

More at [radeksprta.eu](https://radeksprta.eu).
{{/if}}
