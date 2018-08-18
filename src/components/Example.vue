<template>
    <div>
        <div class="top"></div>
        <grid :grid-data="data" :columns="columns" :showCheckbox="showCheckbox" :columnSet="columnSet" :left-height="50" @focus="focus" @updateValue="update" :showRate="true" class="setwidth"></grid>
    </div>
</template>

<script>
import Grid from '../grid'

export default {
    components: {
        Grid,
    },
    data() {
        return {
            columnSet: true,
            showCheckbox: false,
            data: [],
            columns: [
                { title: '1:00', key: 'brandName', width: 50 },
                { title: '2:00', key: 'goodsName', width: 50 },
                { title: '3:00', key: 'sn', width: 50 },
                { title: '4:00', key: 'materialNo', width: 50 },
                { title: '5:00', key: 'unit', width: 50 },
                { title: '6:00', key: 'requiredQuantity', type: 'number', width: 50 },
                { title: '7:00', key: 'customerRemarks', width: 50 },
                { title: '8:00', key: 'purchasePrice', type: 'number', width: 50 },
                { title: '9:00', key: 'salePrice', type: 'number', width: 50 },
                { title: '10:00', width: 50, key: 'shipDesc' },
                { title: '1:00', key: 'brandName1', width: 50 },
                { title: '2:00', key: 'goodsName1', width: 50 },
                { title: '3:00', key: 'sn1', width: 50 },
                { title: '4:00', key: 'materialNo1', width: 50 },
                { title: '5:00', key: 'unit1', width: 50 },
                { title: '6:00', key: 'requiredQuantity1', type: 'number', width: 50 },
                { title: '7:00', key: 'customerRemarks1', width: 50 },
                { title: '8:00', key: 'purchasePrice1', type: 'number', width: 50 },
                { title: '9:00', key: 'salePrice1', type: 'number', width: 50 },
                { title: '10:00', width: 50, key: 'shipDesc1' },
                { title: '1:00', key: 'brandName2', width: 50 },
                { title: '2:00', key: 'goodsName2', width: 50 },
                { title: '3:00', key: 'sn2', width: 50 },
                { title: '4:00', key: 'materialNo2', width: 50 },
                { title: '5:00', key: 'unit2', width: 50 },
                { title: '6:00', key: 'requiredQuantity2', type: 'number', width: 50 },
                { title: '7:00', key: 'customerRemarks2', width: 50 },
                { title: '8:00', key: 'purchasePrice2', type: 'number', width: 50 },
                { title: '9:00', key: 'salePrice2', type: 'number', width: 50 },
                { title: '10:00', width: 50, key: 'shipDesc2' }
            ],
        }
    },
    created() {
        for (let i = 0; i < 100; i += 1) {
            this.data.push({
                brandName: '审核',
                goodsName: '审核',
                sn: '审核',
                materialNo: '审核',
                unit: '审核',
                requiredQuantity: '审核',
                customerRemarks: '审核',
                purchasePrice: '审核',
                salePrice: '审核',
                shipDesc: '审核',
            })
        }
    },
    methods: {
        update(value) {
            // console.log(value) //eslint-disable-line
        },
        focus(value) {
            // console.log(value) //eslint-disable-line
        },
    },
}
</script>

<style>
    .top {
        width: 1187px;
        height: 200px;
        background-color: pink;
    }
    .setwidth {
        width: 1187px;
        height: 500px;
    }
</style>