<template>
    <AssetFormPageWrap>
        <template v-slot:form-section>
            <FormMosaicDefinitionTransaction />
        </template>
        <template v-slot:form-description>
            <div class="asset-description-sub-title">
                {{ $t('mosaic') }}
            </div>
            <div class="asset-description-text">
                {{ $t('mosaic_describe_text') }}
            </div>
            <div class="asset-description-sub-title">
                {{ $t('supply') }}
            </div>
            <div class="asset-description-text">
                {{ $t('flags_supply') }}
            </div>
            <div class="asset-description-sub-title">
                {{ $t('divisibility') }}
            </div>
            <div class="asset-description-text">
                {{ $t('flags_divisibility') }}
            </div>
            <div class="asset-description-sub-title">
                {{ $t('duration_permanent') }}
            </div>
            <div class="asset-description-text">
                {{ $t('flags_duration_permanent') }}
            </div>
            <div class="asset-description-sub-title">
                {{ $t('transferable') }}
            </div>
            <div class="asset-description-text">
                {{ $t('flags_transferable') }}
            </div>
            <div class="asset-description-sub-title">
                {{ $t('variable_supply') }}
            </div>
            <div class="asset-description-text">
                {{ $t('flags_variable_supply') }}
            </div>
            <div class="asset-description-sub-title">
                {{ $t('restrictable') }}
            </div>
            <div class="asset-description-text">
                {{ $t('flags_restrictable') }}
            </div>
        </template>
    </AssetFormPageWrap>
</template>

<script lang="ts">
// external dependencies
import { Component, Vue } from 'vue-property-decorator';

// child components
import AssetFormPageWrap from '@/views/pages/assets/AssetFormPageWrap/AssetFormPageWrap.vue';
import FormMosaicDefinitionTransaction from '@/views/forms/FormMosaicDefinitionTransaction/FormMosaicDefinitionTransaction.vue';

// @ts-ignore
@Component({
    components: { AssetFormPageWrap, FormMosaicDefinitionTransaction },
})
export default class CreateMosaicPage extends Vue {}
</script>
