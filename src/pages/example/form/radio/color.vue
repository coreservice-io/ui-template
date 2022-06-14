<template>
<div class="col-12">
    <h5 class="mb-1 mt-5">#Colors</h5>

    <b-row class="p-3">
        <b-card-text>
            <span>
                To change the color of the radio use the
                <code>.custom-control-{value}</code> for primary, secondary,
                success, danger, info, warning.
            </span>
        </b-card-text>
    </b-row>

    <b-row class="pr-3 pl-3">
        <b-form-radio v-model="Selected" name="some-radio9" value="e" class="custom-control-primary mr-4  ">
            Primary (Default)
        </b-form-radio>
        <b-form-radio v-model="Selected" name="some-radio9" value="ff" class="custom-control-secondary mr-4 ">
            Secondary
        </b-form-radio>
        <b-form-radio v-model="Selected" name="some-radio9" value="g" class="custom-control-success mr-4  ">
            Success
        </b-form-radio>
        <b-form-radio v-model="Selected" name="some-radio9" value="i" class="custom-control-danger mr-4  ">
            Danger
        </b-form-radio>
        <b-form-radio v-model="Selected" name="some-radio9" value="h" class="custom-control-warning mr-4  ">
            Warning
        </b-form-radio>
        <b-form-radio v-model="Selected" name="some-radio9" value="j" class="custom-control-info mr-4  ">
            Info
        </b-form-radio>
    </b-row>
</div>
</template>

<script>
import {
    BFormRadio,
    BRow,
    BCardText
} from "bootstrap-vue";

export default {
    components: {
        BFormRadio,
        BRow,
        BCardText
    },
    data() {
        return {
            Selected: "e",
        };
    },
};
</script>
