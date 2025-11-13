# Cấu hình MCP Server Excel

Repository này chứa cấu hình MCP Server Excel để sử dụng trên nhiều máy tính.

## Cấu hình

File `mcp.json` chứa cấu hình để thêm vào `.cursor/mcp.json` hoặc `~/.cursor/mcp.json`:

```json
{
  "mcpServers": {
    "excel": {
      "command": "cmd",
      "args": [
        "/c",
        "npx",
        "--yes",
        "@negokaz/excel-mcp-server"
      ]
    }
  }
}
```

## Sử dụng

1. Clone repository này:
   ```bash
   git clone https://github.com/NgoSon3868-Quas/Excel-MCP.git
   cd Excel-MCP
   ```

2. Copy nội dung từ `mcp.json` vào file cấu hình MCP của bạn:
   - Windows: `C:\Users\<username>\.cursor\mcp.json`
   - Mac/Linux: `~/.cursor/mcp.json`
   
   Hoặc merge vào file `mcpServers` hiện có của bạn.

3. Khởi động lại Cursor IDE

## Yêu cầu

- Node.js và npm đã được cài đặt
- Package `@negokaz/excel-mcp-server` sẽ được tự động tải khi sử dụng

## Tính năng

MCP Server Excel cung cấp các công cụ để:
- Đọc và ghi dữ liệu Excel
- Định dạng cells và ranges
- Tạo và quản lý sheets
- Xử lý tables trong Excel

## Kiểm tra cấu hình

Sau khi thêm cấu hình và khởi động lại Cursor:
1. Vào Settings > Tools & MCP
2. Kiểm tra trong danh sách "Installed MCP Servers" có `excel` với trạng thái "Ready"
