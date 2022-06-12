<script>
let items;
$: fetch(`http://yunsangmin.com/api/v1/blog/posts`)
    .then(r => r.json())
    .then(data => {
        items = data;
    });

</script>

<section>
    {#if items}
        {#each items as item}
            <p>{item.id}</p>
            <h3>{item.title}</h3>
            <p>{item.text}</p>
            <p>{item.created_at}</p>
            <p>{item.updated_at}</p>
        {/each}
    {/if}
</section>


<style>
    section {
        max-width: 640px;
    }
</style>
