<template>
<div class="col-12 mb-3">
    <b-card header="Simple Cards">
        <div class="row m-1">

            <div class="col-lg-3 mt-1 mb-1">
                <b-media no-body class="icon-card icon-card-secondary mt-1 mb-1">
                    <b-media-aside>
                        <feather-icon size="32" icon="DollarSignIcon" />
                    </b-media-aside>
                    <b-media-body>
                        <h5>Earnings<b-badge class="float-right" v-b-tooltip.hover.left="'credit detail description here xxx xxxx xxxx xxxxx xxx xxxx xxxxxxx xxxxxxxx xxxxxxx'">
                                About </b-badge>
                        </h5>
                        <small>$134514.4</small>
                    </b-media-body>

                </b-media>
            </div>

            <div class="col-lg-3 mt-1 mb-1">
                <b-media no-body class="icon-card icon-card-secondary mt-1 mb-1">
                    <b-media-aside>
                        <feather-icon size="32" icon="ThumbsUpIcon" />
                    </b-media-aside>
                    <b-media-body>
                        <h5>Thumbs<b-badge class="float-right" v-b-tooltip.hover.left="'credit detail description here xxx xxxx xxxx xxxxx xxx xxxx xxxxxxx xxxxxxxx xxxxxxx'">About</b-badge>
                        </h5>
                        <small> 14134</small>
                    </b-media-body>

                </b-media>
            </div>

            <div class="col-lg-3 mt-1 mb-1">
                <b-media no-body class="icon-card icon-card-secondary mt-1 mb-1">
                    <b-media-aside>
                        <feather-icon size="32" icon="EyeIcon" />
                    </b-media-aside>
                    <b-media-body>
                        <h5>Views <b-badge class="float-right" v-b-tooltip.hover.left="'credit detail description here xxx xxxx xxxx xxxxx xxx xxxx xxxxxxx xxxxxxxx xxxxxxx'">About</b-badge>
                        </h5>
                        <small>9831</small>
                    </b-media-body>
                </b-media>
            </div>

            <div class="col-lg-3 mt-1 mb-1">
                <b-media no-body class="icon-card icon-card-secondary mt-1 mb-1">
                    <b-media-aside>
                        <feather-icon size="32" icon="HeartIcon" />
                    </b-media-aside>
                    <b-media-body>
                        <h5>Likes <b-badge class="float-right" v-b-tooltip.hover.left="'credit detail description here xxx xxxx xxxx xxxxx xxx xxxx xxxxxxx xxxxxxxx xxxxxxx'">About</b-badge>
                        </h5>
                        <small>5143413</small>
                    </b-media-body>
                </b-media>
            </div>

        </div>

        <div class="row  m-1">

            <div class="col-lg-3 mt-1 mb-1">
                <b-media no-body class="icon-card icon-card-primary mt-1 mb-1">
                    <b-media-aside>
                        <feather-icon size="22" icon="MailIcon" />
                    </b-media-aside>

                    <b-media-body>
                        <h5>Credit<b-badge variant="primary" class="float-right" v-b-tooltip.hover.left="'credit detail description here xxx xxxx xxxx xxxxx xxx xxxx xxxxxxx xxxxxxxx xxxxxxx'">About</b-badge>
                        </h5>
                        <small>$134514.141114 </small>
                    </b-media-body>

                </b-media>
            </div>

            <div class="col-lg-3 mt-1 mb-1">
                <b-media no-body class="icon-card icon-card-success mt-1 mb-1">
                    <b-media-aside>
                        <feather-icon size="32" icon="MailIcon" />
                    </b-media-aside>
                    <b-media-body>
                        <h5>Credit<b-badge variant="success" class="float-right" v-b-tooltip.hover.left="'credit detail description here xxx xxxx xxxx xxxxx xxx xxxx xxxxxxx xxxxxxxx xxxxxxx'">About</b-badge>
                        </h5>
                        <small>$134514.1411 </small>
                    </b-media-body>

                </b-media>
            </div>

            <div class="col-lg-3 mt-1 mb-1">
                <b-media no-body class="icon-card icon-card-warning mt-1 mb-1">
                    <b-media-aside>
                        <feather-icon size="32" icon="MailIcon" />
                    </b-media-aside>
                    <b-media-body>
                        <h5>Credit<b-badge variant="warning" class="float-right" v-b-tooltip.hover.left="'credit detail description here xxx xxxx xxxx xxxxx xxx xxxx xxxxxxx xxxxxxxx xxxxxxx'">About</b-badge>
                        </h5>
                        <small>$134514.14114</small>
                    </b-media-body>

                </b-media>
            </div>

            <div class="col-lg-3 mt-1 mb-1">
                <b-media no-body class="icon-card icon-card-danger mt-1 mb-1">
                    <b-media-aside>
                        <feather-icon size="32" icon="MailIcon" />
                    </b-media-aside>
                    <b-media-body>
                        <h5>Credit<b-badge variant="danger" class="float-right" v-b-tooltip.hover.left="'credit detail description here xxx xxxx xxxx xxxxx xxx xxxx xxxxxxx xxxxxxxx xxxxxxx'">About</b-badge>
                        </h5>
                        <small>$134514.14</small>
                    </b-media-body>

                </b-media>
            </div>

        </div>
    </b-card>
</div>
</template>

<script>
import {
    BCard,
    BMedia,
    BMediaAside,
    BAvatar,
    BMediaBody,
    BBadge,
    VBTooltip
} from "bootstrap-vue";

export default {
    components: {
        BCard,
        BMedia,
        BMediaAside,
        BAvatar,
        BMediaBody,
        BBadge,
        VBTooltip
    },
};
</script>
