# XeroRuby::Item

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **String** | User defined item code (max length &#x3D; 30) | 
**inventory_asset_account_code** | **String** | The inventory asset account for the item. The account must be of type INVENTORY. The  COGSAccountCode in PurchaseDetails is also required to create a tracked item | 
**name** | **String** | The name of the item (max length &#x3D; 50) | [optional] 
**is_sold** | **Boolean** | Boolean value, defaults to true. When IsSold is true the item will be available on sales transactions in the Xero UI. If IsSold is updated to false then Description and SalesDetails values will be nulled. | [optional] 
**is_purchased** | **Boolean** | Boolean value, defaults to true. When IsPurchased is true the item is available for purchase transactions in the Xero UI. If IsPurchased is updated to false then PurchaseDescription and PurchaseDetails values will be nulled. | [optional] 
**description** | **String** | The sales description of the item (max length &#x3D; 4000) | [optional] 
**purchase_description** | **String** | The purchase description of the item (max length &#x3D; 4000) | [optional] 
**purchase_details** | [**Purchase**](Purchase.md) |  | [optional] 
**sales_details** | [**Purchase**](Purchase.md) |  | [optional] 
**is_tracked_as_inventory** | **Boolean** | True for items that are tracked as inventory. An item will be tracked as inventory if the InventoryAssetAccountCode and COGSAccountCode are set. | [optional] 
**total_cost_pool** | **Float** | The value of the item on hand. Calculated using average cost accounting. | [optional] 
**quantity_on_hand** | **Float** | The quantity of the item on hand | [optional] 
**updated_date_utc** | **DateTime** | Last modified date in UTC format | [optional] 
**item_id** | **String** | The Xero identifier for an Item | [optional] 
**validation_errors** | [**Array&lt;ValidationError&gt;**](ValidationError.md) | Displays array of validation error messages from the API | [optional] 

## Code Sample

```ruby
require 'XeroRuby'

instance = XeroRuby::Item.new(code: null,
                                 inventory_asset_account_code: null,
                                 name: null,
                                 is_sold: null,
                                 is_purchased: null,
                                 description: null,
                                 purchase_description: null,
                                 purchase_details: null,
                                 sales_details: null,
                                 is_tracked_as_inventory: null,
                                 total_cost_pool: null,
                                 quantity_on_hand: null,
                                 updated_date_utc: null,
                                 item_id: null,
                                 validation_errors: null)
```


