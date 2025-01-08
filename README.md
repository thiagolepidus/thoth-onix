# Thoth ONIX

<details>
  <summary>Header</summary>
  
  `Mandatory` `Composite`
    
  File information.
  
<details>
  <summary>Sender</summary>
  
  `Mandatory` `Composite`
  
  Information about the entity sending the file.
  
<details>
  <summary>SenderName</summary>
      
  `Mandatory`
  
  The name of the entity sending the file.
  
</details>

<details>
  <summary>EmailAddress</summary>

  `Mandatory`

  Email address of contact at sending entity.
  
</details>

</details>

<details>
  <summary>SentDateTime</summary>
    
  `Mandatory`
  
  Specifies the date and time when the file is being sent.

  YYYYMMDDThhmmss (Date e time) format recommended.
  
</details>

</details>

<details>
  <summary>Product</summary>
  
  `Mandatory` `Composite` `Repeatable`
  
  Information about the publication.

  Mandatory for each publication in the file; at least one `<Product>` tag should be included per file.
  
<details>
  <summary>RecordReference</summary>

  `Mandatory`

  Identify the information record which you send out about that product.

  **ISBN** recommended.
  
</details>

<details>
  <summary>NotificationType</summary>

  `Mandatory`

  Indicates the type of notification or update which you are sending

  Only code `03` (Notification confirmed on publication) currently available.

</details>

<details>
  <summary>ProductIdentifier</summary>

  `Mandatory` `Composite` `Repeatable`

  An identifier of the product.
    
<details>
  <summary>ProductIDType</summary>
  
  `Mandatory in composite`

  ONIX code specifying the Product Identifier type provided.

  Mandatory in each occurrence of the `<ProductIdentifier>` composite.

  Available codes:
  <table>
    <tr>
      <th>ONIX Code</th>
      <th>Description</th>
    </tr>
    <tr>
      <td>01</td>
      <td>Proprietary</td>
    </tr>
    <tr>
      <td>06</td>
      <td>DOI</td>
    </tr>
    <tr>
      <td>13</td>
      <td>LCCN</td>
    </tr>
    <tr>
      <td>15</td>
      <td>ISBN-13</td>
    </tr>
    <tr>
      <td>23</td>
      <td>OCLC</td>
    </tr>
  </table>
</details>

<details>
  <summary>IDTypeName</summary>
  
  `Optional`
  
  A name which identifies a proprietary identifier.
  
  Must be used when, and only when, the code in the `<ProductIDType>` element indicates a proprietary identifier (ONIX code 01).
  
</details>

<details>
  <summary>IDValue</summary>

  `Mandatory in composite`

  The identifier value of the type specified in the `<ProductIDType>` element.
  
  Mandatory in each occurrence of the `<ProductIdentifier>` composite.
  
</details>

</details>

<details>
  <summary>DescriptiveDetail</summary>

  `Mandatory` `Composite`

  Description of the form and content of a product.

  Mandatory in any `<Product>` record.
  
<details>
  <summary>ProductComposition</summary>

  `Mandatory` `Composite`

  ONIX code which indicates whether a product consists of a single item or multiple items. 
  
  Mandatory in an occurrence of `<DescriptiveDetail>` composite.

  Only `00` (Single-component retail product) currently available.
  
</details>

<details>
  <summary>ProductForm</summary>

  `Mandatory`

  Indicates the primary form of a product.

  Mandatory in an occurrence of `<DescriptiveDetail>` composite.

  Available codes:
  <table>
    <tr>
      <th>ONIX Code</th>
      <th>Description</th>
    </tr>
    <tr>
      <td>AN</td>
      <td>Downloadable and online audio file</td>
    </tr>
    <tr>
      <td>BB</td>
      <td>Hardback</td>
    </tr>
    <tr>
      <td>BC</td>
      <td>Paperback</td>
    </tr>
    <tr>
      <td>EB</td>
      <td>Digital download and online</td>
    </tr>
  </table>
  
</details>

<details>
  <summary>ProductFormDetail</summary>

  `Optional`

  Specifies the digital format.

  Mandatory when specifying a digital `<ProductForm>` (AN and EB).

  Available codes:

  **AN**
  <table>
    <tr>
      <th>ONIX Code</th>
      <th>Description</th>
    </tr>
    <tr>
      <td>A103</td>
      <td>MP3 format</td>
    </tr>
    <tr>
      <td>A104</td>
      <td>WAV format</td>
    </tr>
  </table>

  **EB**
  <table>
    <tr>
      <th>ONIX Code</th>
      <th>Description</th>
    </tr>
    <tr>
      <td>E100</td>
      <td>Other (use to Fiction Book)</td>
    </tr>
    <tr>
      <td>E101</td>
      <td>EPUB</td>
    </tr>
    <tr>
      <td>E104</td>
      <td>DOCX</td>
    </tr>
    <tr>
      <td>E105</td>
      <td>HTML</td>
    </tr>
    <tr>
      <td>E107</td>
      <td>PDF</td>
    </tr>
    <tr>
      <td>E113</td>
      <td>XHTML</td>
    </tr>
    <tr>
      <td>E116</td>
      <td>Amazon Kindle</td>
    </tr>
    <tr>
      <td>E127</td>
      <td>Mobipocket</td>
    </tr>
  </table>
  
</details>

<details>
  <summary>PrimaryContentType</summary>

  `Mandatory`

  Indicates the primary or only content type included in a product.

  Only code `10` (Text eye-readable) currently available.
  
</details>

<details>
  <summary>Measure</summary>

  `Optional` `Composite` `Repeteable`

  Identifies a measurement and its units, specifying the overall dimensions of a product, including packaging.

<details>
  <summary>MeasureType</summary>

  `Mandatory in composite`

  ONIX code indicating the dimension which is specified.
  
  Mandatory in each occurrence of the `<Measure>` composite.

  Available codes:
  <table>
    <tr>
      <th>ONIX Code</th>
      <th>Description</th>
    </tr>
    <tr>
      <td>01</td>
      <td>Height</td>
    </tr>
    <tr>
      <td>02</td>
      <td>Width</td>
    </tr>
    <tr>
      <td>03</td>
      <td>Thickness</td>
    </tr>
    <tr>
      <td>08</td>
      <td>Unit weight</td>
    </tr>
  </table>
  
</details>
<details>
  <summary>Measurement</summary>

  `Mandatory in composite`

  The value representing the `<MeasureType>` dimension in the units specified by `<MeasureUnitCode>`.

  Mandatory in each occurrence of the `<Measure>` composite.
  
</details>
<details>
  <summary>MeasureUnitCode</summary>

  `Mandatory in composite`

  Indicates the measure unit in which dimensions are given.
  
  Mandatory in each occurrence of the `<Measure>` composite.

  Available codes:

  **Height, Width and Thickness**
  <table>
    <tr>
      <th>Value</th>
      <th>Description</th>
    </tr>
    <tr>
      <td>cm</td>
      <td>Centimeters</td>
    </tr>
    <tr>
      <td>mm</td>
      <td>Millimeters</td>
    </tr>
    <tr>
      <td>in</td>
      <td>Inches (US)</td>
    </tr>
  </table>

  **Unit weight**
  <table>
    <tr>
      <th>Value</th>
      <th>Description</th>
    </tr>
    <tr>
      <td>gr</td>
      <td>Grams</td>
    </tr>
    <tr>
      <td>oz</td>
      <td>Ounces (US)</td>
    </tr>
  </table>
  
</details>

</details>

<details>
  <summary>EpubLicense</summary>
  
  `Optional` `Composite`
  
  Name or title of the license governing use of the product, and a link to the license terms in eye-readable or machine-readable form.
  
<details>
  <summary>EpubLicenseName</summary>

  `Mandatory in composite`

  The name or title of the license. 
  
  Mandatory in any `<EpubLicense>` composite.
  
</details>

<details>
  <summary>EpubLicenseExpression</summary>

  `Mandatory in composite` `Composite`

  Details a link to an expression of the license terms.
  
<details>
  <summary>EpubLicenseExpressionType</summary>

  `Mandatory in composite`

  ONIX code identifying the nature or format of the license expression specified.

  Only code `02` (Professional readable) currently available.
  
</details>

<details>
  <summary>EpubLicenseExpressionLink</summary>

  `Mandatory in composite`

  The URI for the license expression.
  
</details>

</details>
</details>
<details>
  <summary>TitleDetail</summary>
  
  `Mandatory` `Composite`

  Title of the product described in the record.
  
<details>
  
  <summary>TitleType</summary>
  
  `Mandatory in composite`

  ONIX code indicating the type of a title.
  
  Only code `02` (Distinctive title (book)) currently available.
  
</details>
<details>
  <summary>TitleElement</summary>

  `Mandatory in composite` `Composite`

  Group of elements representing the title element.
  
<details>
  <summary>TitleElementLevel</summary>

  `Mandatory in composite`

  ONIX code indicating the level of a title element.

  Only code `01` (Product) currently available.
  
</details>

<details>
  <summary>TitleText</summary>

  `Mandatory in composite`

  The text of a title element, excluding any subtitle.
  
</details>
<details>
  <summary>Subtitle</summary>

  `Optional`

  The text of a subtitle.
  
</details>

</details>

</details>

<details>
<summary>Contributor</summary>
<details>
<summary>SequenceNumber</summary>
</details>
<details>
<summary>ContributorRole</summary>
</details>
<details>
<summary>NameIdentifier</summary>
<details>
<summary>NameIDType</summary>
</details>
<details>
<summary>IDValue</summary>
</details>
</details>
<details>
<summary>PersonName</summary>
</details>
<details>
<summary>NamesBeforeKey</summary>
</details>
<details>
<summary>KeyNames</summary>
</details>
<details>
<summary>ProfessionalAffiliation</summary>
<details>
<summary>ProfessionalPosition</summary>
</details>
<details>
<summary>Affiliation</summary>
</details>
</details>
<details>
<summary>BiographicalNote</summary>
</details>
<details>
<summary>Website</summary>
<details>
<summary>WebsiteRole</summary>
</details>
<details>
<summary>WebsiteDescription</summary>
</details>
<details>
<summary>WebsiteLink</summary>
</details>
</details>
</details>
<details>
<summary>Edition</summary>
<details>
<summary>EditionNumber</summary>
</details>
</details>
<details>
<summary>Language</summary>
<details>
<summary>LanguageRole</summary>
</details>
<details>
<summary>LanguageCode</summary>
</details>
</details>
<details>
<summary>Extent</summary>
<details>
<summary>ExtentType</summary>
</details>
<details>
<summary>ExtentValue</summary>
</details>
<details>
<summary>ExtentUnit</summary>
</details>
</details>
<details>
<summary>IllustrationsNote</summary>
</details>
<details>
<summary>AncillaryContent</summary>
<details>
<summary>AncillaryContentType</summary>
</details>
<details>
<summary>AncillaryContentDescription</summary>
</details>
<details>
<summary>Number</summary>
</details>
</details>
<details>
<summary>Subject</summary>
<details>
<summary>MainSubject</summary>
</details>
<details>
<summary>SubjectSchemeIdentifier</summary>
</details>
<details>
<summary>SubjectHeadingText</summary>
</details>
<details>
<summary>SubjectCode</summary>
</details>
</details>
<details>
<summary>Audience</summary>
<details>
<summary>AudienceCodeType</summary>
</details>
<details>
<summary>AudienceCodeValue</summary>
</details>
</details>
</details>
<details>
<summary>CollateralDetail</summary>
<details>
<summary>TextContent</summary>
<details>
<summary>TextType</summary>
</details>
<details>
<summary>ContentAudience</summary>
</details>
<details>
<summary>Text</summary>
</details>
</details>
<details>
<summary>SupportingResource</summary>
<details>
<summary>ResourceContentType</summary>
</details>
<details>
<summary>ContentAudience</summary>
</details>
<details>
<summary>ResourceMode</summary>
</details>
<details>
<summary>ResourceFeature</summary>
<details>
<summary>ResourceFeatureType</summary>
</details>
<details>
<summary>FeatureNote</summary>
</details>
</details>
<details>
<summary>ResourceVersion</summary>
<details>
<summary>ResourceForm</summary>
</details>
<details>
<summary>ResourceLink</summary>
</details>
</details>
</details>
</details>
<details>
<summary>ContentDetail</summary>
<details>
<summary>ContentItem</summary>
<details>
<summary>LevelSequenceNumber</summary>
</details>
</details>
<details>
<summary>TextItem</summary>
<details>
<summary>TextItemType</summary>
</details>
<details>
<summary>TextItemIdentifier</summary>
<details>
<summary>TextItemIDType</summary>
</details>
<details>
<summary>IDValue</summary>
</details>
</details>
</details>
<details>
<summary>PageRun</summary>
<details>
<summary>FirstPageNumber</summary>
</details>
<details>
<summary>LastPageNumber</summary>
</details>
</details>
<details>
<summary>NumberOfPages</summary>
</details>
</details>
<details>
<summary>PublishingDetail</summary>
<details>
<summary>Imprint</summary>
<details>
<summary>ImprintName</summary>
<details>
<summary>ImprintIdentifier</summary>
<details>
<summary>ImprintIDType</summary>
</details>
<details>
<summary>IDTypeName</summary>
</details>
<details>
<summary>IDValue</summary>
</details>
</details>
</details>
</details>
<details>
<summary>Publisher</summary>
<details>
<summary>PublishingRole</summary>
</details>
<details>
<summary>PublisherIdentifier</summary>
<details>
<summary>PublisherIDType</summary>
</details>
<details>
<summary>IDValue</summary>
</details>
</details>
<details>
<summary>PublisherName</summary>
</details>
<details>
<summary>Website</summary>
<details>
<summary>WebsiteRole</summary>
</details>
<details>
<summary>WebsiteDescription</summary>
</details>
<details>
<summary>WebsiteLink</summary>
</details>
</details>
<details>
<summary>Funding</summary>
<details>
<summary>FundingIdentifier</summary>
<details>
<summary>FundingIDType</summary>
</details>
<details>
<summary>IDTypeName</summary>
</details>
<details>
<summary>IDValue</summary>
</details>
</details>
</details>
</details>
<details>
<summary>CityOfPublication</summary>
</details>
<details>
<summary>PublishingStatus</summary>
</details>
<details>
<summary>PublishingDate</summary>
<details>
<summary>PublishingDateRole</summary>
</details>
<details>
<summary>Date</summary>
</details>
</details>
<details>
<summary>CopyrightStatement</summary>
<details>
<summary>CopyrightOwner</summary>
<details>
<summary>PersonName</summary>
</details>
</details>
</details>
<details>
<summary>SalesRights</summary>
<details>
<summary>SalesRightsType</summary>
</details>
<details>
<summary>Territory</summary>
<details>
<summary>RegionsIncluded</summary>
</details>
</details>
</details>
</details>
<details>
<summary>RelatedMaterial</summary>
<details>
<summary>RelatedWork</summary>
<details>
<summary>WorkRelationCode</summary>
</details>
<details>
<summary>WorkIdentifier</summary>
<details>
<summary>WorkIDType</summary>
</details>
<details>
<summary>IDValue</summary>
</details>
</details>
</details>
<details>
<summary>RelatedProduct</summary>
<details>
<summary>ProductRelationCode</summary>
</details>
<details>
<summary>ProductIdentifier</summary>
<details>
<summary>ProductIDType</summary>
</details>
<details>
<summary>IDTypeName</summary>
</details>
<details>
<summary>IDValue</summary>
</details>
</details>
</details>
</details>
<details>
<summary>ProductSupply</summary>
<details>
<summary>Market</summary>
<details>
<summary>Territory</summary>
<details>
<summary>RegionsIncluded</summary>
</details>
</details>
</details>
<details>
<summary>SupplyDetail</summary>
<details>
<summary>Supplier</summary>
<details>
<summary>SupplierRole</summary>
</details>
<details>
<summary>SupplierName</summary>
</details>
<details>
<summary>Website</summary>
<details>
<summary>WebsiteRole</summary>
</details>
<details>
<summary>WebsiteDescription</summary>
</details>
<details>
<summary>WebsiteLink</summary>
</details>
</details>
</details>
<details>
<summary>ProductAvailability</summary>
</details>
<details>
<summary>SupplyDate</summary>
<details>
<summary>SupplyDateRole</summary>
</details>
</details>
<details>
<summary>UnpricedItemType</summary>
</details>
<details>
<summary>Price</summary>
<details>
<summary>PriceType</summary>
</details>
<details>
<summary>PriceAmount</summary>
</details>
<details>
<summary>CurrencyCode</summary>
</details>
<details>
<summary>Territory</summary>
<details>
<summary>RegionsIncluded</summary>
</details>
</details>
</details>
</details>
</details>
</details>
