<template>
    <div>
        <fieldset class="mb-4">
            <legend>General Information</legend>
            <div class="row">
                <div class="col-md-6">
                    <div class="form-group row mb-2 mb-md-0 text-only">
                        <label class="col-md-4 col-form-label text-md-right">
                            Name
                        </label>
                        <div class="col-md-8">
                            <dsp-text v-model="record.name" />
                        </div>
                    </div>
                    <div class="form-group row mb-2 mb-md-0 text-only">
                        <label class="col-md-4 col-form-label text-md-right">
                            Deleted At
                        </label>
                        <div class="col-md-8">
                            <dsp-text v-model="record.deleted_at" />
                        </div>
                    </div>
                </div>
            </div>
        </fieldset>
    </div>
</template>

<script>
export default {
    name: "service-type-show",
    props: {
        record: {
            type: [Boolean, Object],
            default: false
        }
    }
};
</script>
