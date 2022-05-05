<script>
    // your script goes here
</script>

<svelte:head>
    <title>Hello</title>
</svelte:head>

<!-- <div class="section">
    <div class="container">
        <h1 class="title">Hello World</h1>
        <p class="subtitle">Hello again!</p>
    </div>
</div> -->

<div class="section pb-4">
    <div class="columns">
        <div class="column is-one-quarter py-1">
            <div class="box" id="orderBox" />
        </div>
        <div class="column is-half">
            <div class="box">
                <div class="columns is-multiline">
                    {#each Array(9) as _, i}
                        <div class="column is-one-fifth p-1">
                            <button
                                class="button is-responsive is-large is-clipped is-black is-fullwidth"
                                >Press me!</button
                            >
                        </div>
                    {/each}
                </div>
            </div>
            <div class="columns is-multiline">
                {#each Array(15) as _, i}
                    <div class="column is-one-fifth p-1">
                        {#if i % 7 != 0}
                            <button
                                class="button is-responsive is-large is-clipped is-fullwidth {i %
                                    8 ==
                                0
                                    ? 'is-primary'
                                    : ''}">Press me!</button
                            >
                        {/if}
                    </div>
                {/each}
            </div>
        </div>
        <div class="column is-one-quarter py-1">
            <div class="box" id="recentOrders" />
        </div>
    </div>
</div>

<div class="section pt-4">
    <div class="columns">
        <div class="column is-one-quarter py-1">
            <div class="box" id="customization">
                <div class="columns is-multiline">
                    {#each Array(15) as _, i}
                        <div class="column is-one-third p-1">
                            <button
                                class="button is-responsive is-large is-clipped is-fullwidth"
                                >Press me!</button
                            >
                        </div>
                    {/each}
                </div>
            </div>
        </div>
        <div class="column is-half">
            <div class="columns is-multiline">
                {#each Array(25) as _, i}
                    <div class="column is-one-fifth p-1">
                        {#if i % 7 != 0}
                            <button
                                class="button is-responsive is-large is-clipped is-fullwidth {i %
                                    8 ==
                                0
                                    ? 'is-primary'
                                    : ''}">Press me!</button
                            >
                        {/if}
                    </div>
                {/each}
            </div>
        </div>
        <div class="column is-one-quarter py-1">
            <div class="box" id="payMenu">
                <div class="columns is-multiline">
                    {#each Array(20) as _, i}
                        <div class="column is-one-quarter p-1">
                            <button
                                class="button is-responsive is-large is-dark is-clipped is-fullwidth"
                                >Press me!</button
                            >
                        </div>
                    {/each}
                </div>
            </div>
        </div>
    </div>
</div>

<style>
    #orderBox {
        height: 100%;
    }

    #recentOrders {
        height: 100%;
    }

    #payMenu {
        overflow-wrap: break-word;
    }
</style>
