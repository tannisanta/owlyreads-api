The changelog lists all updates, enhancements, and removals in the API.

<script>
    function toggleAccordion(button) {
        const panel = button.nextElementSibling;
        const isOpen = panel.style.display === 'block';
        panel.style.display = isOpen ? 'none' : 'block';
        button.children[0].style.transform = isOpen ? 'rotate(-90deg)' : 'rotate(0deg)';
    }
    function safeText(value) {
        if (value === null || value === undefined) return '';
        return typeof value === 'string' ? value : JSON.stringify(value);
    }
</script>
<!-- API change impact section -->
<div style="margin-top: 20px;">
    <button onclick="toggleAccordion(this)" style="background-color: #eee; color: #444; cursor: pointer; padding: 18px; width: 100%; border: none; text-align: left; outline: none; font-size: 15px; position: relative;">
        <div style="width: 0; height: 0; border-left: 5px solid transparent; border-right: 5px solid transparent; border-bottom: 5px solid #444; position: absolute; right: 10px; top: 50%; transform: translateY(-50%) rotate(-90deg); transition: transform 0.4s;"></div>
        <b>API change impact</b>
    </button>
    <div style="padding: 0 18px; background-color: #fff; display: none; overflow: hidden;">
        <p>Changes to the <strong>OwlyReads Catalog API</strong> aim to minimize disruption. Some adjustments may be required depending on the change type.</p>
        <div style="font-size: 0.9em; background-color: #f9f9f9; padding: 12px; border-left: 4px solid #ccc; margin-top: 16px;">
            <p>Deprecated fields or features in the changelog serve as early notice. They will not be removed immediately but should be avoided in new integrations.</p>
        </div>
        <p><b>Non-breaking changes</b></p>
        <ul>
            <li><strong>Requests:</strong> Adding optional fields or changing required fields to optional.</li>
            <li><strong>Responses:</strong> Adding optional fields or changing optional fields to required.</li>
            <li><strong>Headers:</strong> Adding optional headers or adjusting header name case.</li>
            <li><strong>Field length:</strong> Expanding maximum length of existing fields.</li>
            <li><strong>Identifier format:</strong> Adjusting prefixes or identifier formatting.</li>
            <li><strong>Webhooks:</strong> Adding new event types (opt-in) or new payload fields.</li>
            <li><strong>Rate limiting:</strong> Announced at least one month in advance.</li>
        </ul>
        <p><b>Breaking changes</b></p>
        <ul>
            <li><strong>Operation removal:</strong> Removing an API operation.</li>
            <li><strong>Requests:</strong> Removing/renaming fields, making optional fields required, removing <code>oneOf</code>.</li>
            <li><strong>Responses:</strong> Removing/renaming fields, changing status codes, removing <code>oneOf</code>.</li>
            <li><strong>Type changes:</strong> Changing field data type.</li>
            <li><strong>Headers:</strong> Adding/removing required headers.</li>
            <li><strong>Enums:</strong> Adding/removing enum values.</li>
            <li><strong>Errors:</strong> Changing error codes.</li>
            <li><strong>Validation:</strong> Adding stricter rules.</li>
            <li><strong>Auth:</strong> Changing authentication or authorization requirements.</li>
        </ul>
    </div>
</div>
<br>
<!-- Monthly changelog entries -->
<div style="margin-top: 30px;">
    <button onclick="toggleAccordion(this)" style="background-color: #eee; color: #444; cursor: pointer; padding: 18px; width: 100%; border: none; text-align: left; outline: none; font-size: 15px; position: relative;">
        <div style="width: 0; height: 0; border-left: 5px solid transparent; border-right: 5px solid transparent; border-bottom: 5px solid #444; position: absolute; right: 10px; top: 50%; transform: translateY(-50%) rotate(0deg); transition: transform 0.4s;"></div>
        <b>2025</b>
    </button>
    <div style="padding: 0 18px; background-color: #fff; display: block; overflow: hidden;">
<!-- 27 September -->
<p><strong>27 September 2025</strong></p>
<table style="table-layout: fixed; border-collapse: collapse; width: 100%; border: none;">
    <tr>
        <td style="width: 25%; vertical-align: top; padding-right: 10px; border: none;">
            <svg xmlns="http://www.w3.org/2000/svg" width="65" height="20" viewBox="0 0 65 20">
                <rect x="1" y="1" width="63" height="18" rx="4" fill="none" stroke="#308132" stroke-width="1"></rect>
                <text x="32" y="14" font-size="12" fill="#308132" font-family="Arial, sans-serif" font-weight="lighter" text-anchor="middle">Added</text>
            </svg>
        </td>
        <td style="width: 75%; vertical-align: top; border: none;">
            <code>currency</code> field to the requests and responses of the Books section.
        </td>
    </tr>
</table>
<!-- 5 August -->
<p><strong>5 August 2025</strong></p>
<table style="table-layout: fixed; border-collapse: collapse; width: 100%; border: none;">
    <tr>
        <td style="width: 25%; vertical-align: top; padding-right: 10px; border: none;">
            <svg xmlns="http://www.w3.org/2000/svg" width="65" height="20" viewBox="0 0 65 20">
                <rect x="1" y="1" width="63" height="18" rx="4" fill="none" stroke="#308132" stroke-width="1"></rect>
                <text x="32" y="14" font-size="12" fill="#308132" font-family="Arial, sans-serif" font-weight="lighter" text-anchor="middle">Added</text>
            </svg>
        </td>
        <td style="width: 75%; vertical-align: top; border: none;">
            <code>availability</code> field to indicate whether the book is in stock in all operations related to books.
        </td>
    </tr>
</table>
