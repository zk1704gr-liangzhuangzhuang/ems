<template>
	<view>
		<view class="div-table">
			<view class="thead">
				<view class="th">
					<view class="td">设备名称</view>
					<view class="td">故障原因</view>
					<view class="td">报告人</view>
					<view class="td">故障时间(分钟)</view>
				</view>
			</view>
			<view class="tr">
				<view class="td">zk-1#斗轮机</view>
				<view class="td">轻断裂</view>
				<view class="td">东猫猫</view>
				<view class="td">30</view>
			</view>
			<view class="tr">
				<view class="td">zk-2#斗轮机</view>
				<view class="td">突然断电</view>
				<view class="td">于合壁</view>
				<view class="td">40</view>
			</view>
			<view class="tr">
				<view class="td">zk-3#斗轮机</view>
				<view class="td">自然原因(风)</view>
				<view class="td">党刘涛</view>
				<view class="td">50</view>
			</view>
			<view class="tr">
				<view class="td">zk-4#斗轮机</view>
				<view class="td">卡东西</view>
				<view class="td">柴年年</view>
				<view class="td">10</view>
			</view>
		</view>
	</view>
</template>

<script>
export default {
	data() {
		return {
			
		};
	}
};
</script>

<style lang="scss">
$div-table-border-color: #666;
$div-table-border-width: 1upx;

.div-table {
	display: table;
	width: 100%;
	height: 100%;
	border-top: $div-table-border-width solid $div-table-border-color;
	border-bottom: $div-table-border-width solid $div-table-border-color;
	box-sizing: border-box;
	table-layout: fixed;
	position: relative;
	.celspan {
		display: table;
		width: 100%;
		height: 100%;
		.td {
			display: table-cell;
			border: none !important;
		}
		.td + .td {
			border-left: $div-table-border-width solid $div-table-border-color !important;
		}
	}
	.rowspan {
		display: table;
		width: 100%;
		height: 100%;
		.tr {
			display: table-row;
			border: none !important;
		}
	}

	&.fixed-thead {
		.tbody,
		.thead,
		.tr,
		.th,
		.td {
			display: block;
		}
		.tr,
		.th {
			&:after {
				content: '';
				display: block;
				visibility: hidden;
				clear: both;
				height: 0;
			}
		}
		.td {
			float: left;
			width: 33.33%;
		}
		.tbody {
			height: 400upx;
			overflow-y: auto;
			overflow-x: hidden;
		}
	}

	.tr,
	.th {
		display: table-row;
		& + .tr,
		& + .th {
			.td,
			.th {
				border-top: $div-table-border-width solid $div-table-border-color;
				word-break: break-word;
			}
		}
	}
	.rowspan {
		.tr,
		.th {
			display: table-row;
			.td,
			.th {
				border: none;
			}
			& + .tr,
			& + .th {
				.td,
				.th {
					border-top: $div-table-border-width solid $div-table-border-color;
				}
			}
		}
	}
	.td {
		display: table-cell;
		vertical-align: middle;
		text-align: center;
		box-sizing: border-box;
		padding: 30upx;
		&.noPadding {
			padding: 0;
		}
		& + .td {
			border-left: $div-table-border-width solid $div-table-border-color;
		}
	}
	.th .td {
		font-weight: bold;
	}
	.tbody {
		display: table-row-group;
	}
	.thead {
		display: table-header-group;
		.tr,
		.th {
			.td,
			.th {
				border-bottom: $div-table-border-width solid $div-table-border-color;
			}
		}
	}
	.tfoot {
		display: table-footer-group;
		.tr,
		.th {
			.td,
			.th {
				border-top: $div-table-border-width solid $div-table-border-color;
			}
		}
	}
	.colgroup {
		display: table-column-group;
	}
	.col {
		display: table-column;
	}
	.caption {
		display: table-caption;
	}
}
</style>
