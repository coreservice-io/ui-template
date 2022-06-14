<template>
<div class="col-12 mb-5">
    <h5 class="mb-3 mt-5">#Custom</h5>
        <b-list-group>
            <b-list-group-item active>
                <div class="d-flex w-100 justify-content-between mb-1">
                    <h5 class="mb-1">
                        List group item heading
                    </h5>
                    <small>3 days ago</small>
                </div>
                <b-card-text>
                    <p class="mb-2"> Donec id elit non mi porta gravida at eget metus. Maecenas sed diam eget risus varius blandit.</p>
                    <small>Donec id elit non mi porta.</small>
                </b-card-text>

            </b-list-group-item>

            <b-list-group-item >
                <div class="d-flex w-100 justify-content-between mb-1">
                    <h5 class="mb-1">
                        List group item heading
                    </h5>
                    <small>3 days ago</small>
                </div>
                <b-card-text class="mb-1">
                    <p class="mb-2"> Donec id elit non mi porta gravida at eget metus. Maecenas sed diam eget risus varius blandit.</p>
                    <small>Donec id elit non mi porta.</small>
                </b-card-text>

            </b-list-group-item>

            <b-list-group-item >
                <div class="d-flex w-100 justify-content-between mb-1">
                    <h5 class="mb-1">
                        List group item heading
                    </h5>
                    <small>3 days ago</small>
                </div>
                <b-card-text class="mb-1">
                    <p class="mb-2"> Donec id elit non mi porta gravida at eget metus. Maecenas sed diam eget risus varius blandit.</p>
                    <small>Donec id elit non mi porta.</small>
                </b-card-text>

            </b-list-group-item>

        </b-list-group>
</div>
</template>

<script>
import {
    BListGroup,
    BListGroupItem,
    BCardText
} from "bootstrap-vue";

export default {
    components: {
        BListGroup,
        BListGroupItem,
        BCardText
    },
};
</script>
