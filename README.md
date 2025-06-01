### `createPage(databaseId, properties)`

**Parameters:**  
- `databaseId` (string) — Notion database ID  
- `properties` (object) — Properties object following the Notion API format for the new page  

**Returns:**  
- Promise resolving to the created page object  

**Description:**  
Creates a new page in the specified database with given property values.  

---

### `appendBlockChildren(blockId, children)`

**Parameters**

- `blockId` (string) — ID of the parent block or page to append children to  
- `children` (Array<Object>) — Array of block objects created by block builder functions  

**Returns**  
Promise resolving to the Notion API response containing the updated block children  

**Description**  
Appends child blocks to a specified block or page by calling the Notion API PATCH endpoint  
`/v1/blocks/{blockId}/children`.


