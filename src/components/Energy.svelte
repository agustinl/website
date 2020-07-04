<script>
    import { _ } from 'svelte-i18n';
</script>

<div class="scene energy">
    <div class="text">
        <div class="container">
            <div class="text__inside">
                <p class="subtitle">{@html $_('energy.sub')}</p>
                <h2 class="title">
                    {@html $_('energy.title')}
                </h2>
                <div class="lead">
                    <p>{@html $_('energy.lead')}</p>
                </div>
            </div>
        </div>
    </div>
</div>

<style>
.energy {
    display: flex;
    align-items: flex-start;
    flex-direction: column;
    position: relative;
    background: none;
    overflow: hidden;
    z-index: 5;
}
.energy .text {
    top: 18.7vh;
}
.energy .text .container {
    margin-left: 11vw;
}
</style>