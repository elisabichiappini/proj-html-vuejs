<script>
export default {
    name: 'CardsNewLetterComponents',
};
</script>

<template>
    <section id="newletter">
        <div class="container">
            <ul class="col d-flex gap-4 justify-content-center align-items-center">
                <li class="box-icon">
                    <font-awesome-icon icon="fa-regular fa-envelope" />
                </li>
                <li class="text-subscription">Subscribe now and get special offert</li>
                <li class="ec-input-text">
                    <label for="inputMail"></label>
                    <input type="text" class="rounded-pill" id="inputMail" placeholder="Insert your email">
                </li>
                <li class="nav-item text-uppercase">
                    <a class="nav-link ec-color-primary rounded-pill px-5" aria-current="page" href="#">Send</a>
                </li>
            </ul>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../assets/styles/partials/variables' as *;
#newletter {
    background-color:$footer-top;
    padding: 80px 0;
    ul {
        all:unset;
        list-style-type: none;
        .box-icon {
            color: $elements;
            padding: 9px 13px;
            border-radius: 40px;
            background-color: $text;
            font-size: 24px;
        }
        .text-subscription {
            font-weight: 800;
            font-size: 20px;
            color: $white;
        }
        input {
            padding: 0 100px 0 16px;
        }
        .ec-color-primary {
            background-color: $color-primary;
            color: $white;
            &:hover {
                background-color: $color-secondary;
                color: $white;
            }
        }
       
    }
    
}

</style>