<template>
<div class="col-12 mb-5">
    <b-card header="Forms">
        <div class="p-3">
            <b-button  class="mr-3 "  v-b-modal.modal-login variant="primary">
                Login Form
            </b-button>

            <!-- modal scrolling content button -->
            <b-button  class="mr-3 " v-b-modal.modal-tall variant="primary">
                Scrolling Long Content
            </b-button>

            <!-- button Scrolling Content inside Modal-->
            <b-button  class="mr-3 " v-b-modal.modal-scrollable variant="primary">
                Scrolling Content inside Modal
            </b-button>

            <!-- select 2 demo -->
            <b-button  class="mr-3 " v-b-modal.modal-select2 variant="primary">
                Select2 With Modal
            </b-button>

            <!-- modal login-->
            <b-modal id="modal-login" cancel-variant="secondary" ok-title="Login" cancel-title="Close" centered title="Login Form">
                <b-form>
                    <b-form-group>
                        <label for="email">Email:</label>
                        <b-form-input id="email" type="email" placeholder="Email Address" />
                    </b-form-group>
                    <b-form-group>
                        <label for="password">Password</label>
                        <b-form-input type="password" placeholder="Password" />
                    </b-form-group>
                </b-form>
            </b-modal>

            <!-- modal scrolling content -->
            <b-modal id="modal-tall" title="Overflowing Content" cancel-variant="secondary" cancel-title="Close" ok-title="Accept">
                <b-card-text v-for="(content,index) in scrollContent" :key="index">
                    {{ content }}
                </b-card-text>
            </b-modal>

            <!-- modal Scrolling Content inside Modal-->
            <b-modal id="modal-scrollable" scrollable title="Scrollable Content" cancel-title="Close" ok-title="Accept" cancel-variant="secondary">
                <b-card-text v-for="(content,index) in scrollContent" :key="index">
                    {{ content }}
                </b-card-text>
            </b-modal>

            <!-- select 2 demo -->
            <b-modal id="modal-select2" title="Basic Modal" ok-title="submit" cancel-variant="secondary">
                <b-form>
                    <b-form-group label="Enter Name" label-for="name">
                        <b-form-input id="name" placeholder="Enter name" />
                    </b-form-group>
                    <b-form-group label="Choose the country" label-for="vue-select">
                        <v-select id="vue-select" v-model="selected" :options="option" />
                    </b-form-group>
                    <b-form-group label="Zip Code" label-for="zip-code">
                        <b-form-input id="zip-code" type="number" placeholder="Zip Code" />
                    </b-form-group>
                </b-form>
            </b-modal>
        </div>    
    </b-card>
</div>
</template>

<script>
import {
    BCard,
    BButton,
    BAlert,
    BForm,
    BFormInput,
    BFormGroup,
    BCardText
} from "bootstrap-vue";

import vSelect from 'vue-select'

export default {
    components: {
        BCard,
        BButton,
        BAlert,
        BForm,
        BFormInput,
        BFormGroup,
        BCardText,
        vSelect
    },

    data() {
        return {
            scrollContent: [
                'Biscuit powder jelly beans. Lollipop candy canes croissant icing chocolate cake. Cake fruitcake powder pudding pastry.',
                'Tootsie roll oat cake I love bear claw I love caramels caramels halvah chocolate bar. Cotton candy gummi bears pudding pie apple pie cookie. Cheesecake jujubes lemon drops danish dessert I love caramels powder.',
                'Chocolate cake icing tiramisu liquorice toffee donut sweet roll cake. Cupcake dessert icing dragée dessert. Liquorice jujubes cake tart pie donut. Cotton candy candy canes lollipop liquorice chocolate marzipan muffin pie liquorice.',
                'Powder cookie jelly beans sugar plum ice cream. Candy canes I love powder sugar plum tiramisu. Liquorice pudding chocolate cake cupcake topping biscuit. Lemon drops apple pie sesame snaps tootsie roll carrot cake soufflé halvah. Biscuit powder jelly beans. Lollipop candy canes croissant icing chocolate cake. Cake fruitcake powder pudding pastry.',
                'Tootsie roll oat cake I love bear claw I love caramels caramels halvah chocolate bar. Cotton candy gummi bears pudding pie apple pie cookie. Cheesecake jujubes lemon drops danish dessert I love caramels powder.',
                'Chocolate cake icing tiramisu liquorice toffee donut sweet roll cake. Cupcake dessert icing dragée dessert. Liquorice jujubes cake tart pie donut. Cotton candy candy canes lollipop liquorice chocolate marzipan muffin pie liquorice.',
                'Powder cookie jelly beans sugar plum ice cream. Candy canes I love powder sugar plum tiramisu. Liquorice pudding chocolate cake cupcake topping biscuit. Lemon drops apple pie sesame snaps tootsie roll carrot cake soufflé halvah. Biscuit powder jelly beans. Lollipop candy canes croissant icing chocolate cake. Cake fruitcake powder pudding pastry.',
                'Tootsie roll oat cake I love bear claw I love caramels caramels halvah chocolate bar. Cotton candy gummi bears pudding pie apple pie cookie. Cheesecake jujubes lemon drops danish dessert I love caramels powder.',
                'Chocolate cake icing tiramisu liquorice toffee donut sweet roll cake. Cupcake dessert icing dragée dessert. Liquorice jujubes cake tart pie donut. Cotton candy candy canes lollipop liquorice chocolate marzipan muffin pie liquorice.',
                'Powder cookie jelly beans sugar plum ice cream. Candy canes I love powder sugar plum tiramisu. Liquorice pudding chocolate cake cupcake topping biscuit. Lemon drops apple pie sesame snaps tootsie roll carrot cake soufflé halvah. Biscuit powder jelly beans. Lollipop candy canes croissant icing chocolate cake. Cake fruitcake powder pudding pastry.',
                'Tootsie roll oat cake I love bear claw I love caramels caramels halvah chocolate bar. Cotton candy gummi bears pudding pie apple pie cookie. Cheesecake jujubes lemon drops danish dessert I love caramels powder.',
                'Chocolate cake icing tiramisu liquorice toffee donut sweet roll cake. Cupcake dessert icing dragée dessert. Liquorice jujubes cake tart pie donut. Cotton candy candy canes lollipop liquorice chocolate marzipan muffin pie liquorice.',
                'Powder cookie jelly beans sugar plum ice cream. Candy canes I love powder sugar plum tiramisu. Liquorice pudding chocolate cake cupcake topping biscuit. Lemon drops apple pie sesame snaps tootsie roll carrot cake soufflé halvah.',
            ],
            selected: 'USA',
            option: ['USA', 'Canada', 'Maxico'],
        }
    }
};
</script>
