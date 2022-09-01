<script>
    import Comments from "./Coments.svelte";
</script>
<div class="Card">
    <div class="Card-container">
        <div class="Card-header">
            <div class="Card-user">
                <img src="" alt="" />
                <h2>Elmo.pug<span>Bogota, Colombia</span></h2>
            </div>
            <div class="Card-settings">
                <i class="fa-solid fa-ellipsis-vertical"></i>
            </div>
        </div>
        <div class="Card-photo">
            <figure>
                <img src="" alt="" />
            </figure>
        </div>
        <div class="Card-icons">
            <div class="Card-icon-first">
                <i class="fa-solid fa-heart"></i>
                <i class="fa-duotone fa-plane"></i>
            </div>
            <div class="Card-icons-second">
                <i class="fa-solid fa-bookmark"></i>
            </div>
        </div>
        <div class="Card-description">
            <h3>Elmo.pug</h3>
            <span>Hola</span>
        </div>
        <Comments />
    </div>
</div>