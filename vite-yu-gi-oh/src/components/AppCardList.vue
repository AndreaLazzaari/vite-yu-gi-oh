<template lang="">
    <div class='my-container p-5'>
        <div class='container'>
            <div class='row'>
                <article class='col-6 col-md-4 col-lg-3'>
                    <div class="card">
                        <img src="..." class="card-img-top" alt="...">
                        <div class="card-body">
                            <h5 class="card-title">Card title</h5>
                            <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
                        </div>
                        <ul class="list-group list-group-flush">
                            <li class="list-group-item">An item</li>
                        </ul>
                    </div>
                </article>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
@use '../styles/general.scss' as *;

    div.my-container{
        width: 85%;
        height: 100%;
        margin: 0 auto;
        background-color: red;
        margin-top: 4rem;
    }
</style>