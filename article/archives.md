template: default
---

<div class="pure-table">


<ul class="archives">
: for $blog.entries() -> $entry {
<li><time><: $entry.published_at.strftime('%Y-%m-%d') :></time>　<a href="<: $entry.site_path() | uri_for :>"><: $entry.title :></a></li>
: }
</ul>

</div>
