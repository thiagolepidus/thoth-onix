# Thoth ONIX

<details>
    <summary>Header</summary>
    <table>
        <tr>
            <td>File information</td>
        </tr>
        <tr>
            <td>Required</td>
        </tr>
    </table>
    <details>
        <summary>Sender</summary>
        <table>
            <tr>
                <td>Information about the entity sending the file</td>
            </tr>
            <tr>
                <td>Required</td>
            </tr>
        </table>
        <details>
            <summary>SenderName</summary>
            <table>
                <tr>
                    <td>The name of the entity sending the file</td>
                </tr>
                <tr>
                    <td>Required</td>
                </tr>
            </table>
        </details>
        <details>
            <summary>EmailAddress</summary>
            <table>
                <tr>
                    <td>Email address of contact at sending entity</td>
                </tr>
                <tr>
                    <td>Required</td>
                </tr>
            </table>
        </details>
    </details>
    <details>
        <summary>SentDateTime</summary>
        <table>
            <tr>
                <td>Specifies the date and time when the file is being sent.<br>
                YYYYMMDDThhmmss (Date e time) format recommended</td>
            </tr>
            <tr>
                <td>Required</td>
            </tr>
        </table>
    </details>
</details>
<details>
    <summary>Product</summary>
    <table>
        <tr>
            <td>Information about the publication</td>
        </tr>
        <tr>
            <td>Required, repeatable</td>
        </tr>
    </table>
    <details>
        <summary>RecordReference</summary>
        <table>
            <tr>
                <td>Unique and permanent identifier the record information</td>
            </tr>
            <tr>
                <td>Required</td>
            </tr>
        </table>
    </details>
    <details>
        <summary>NotificationType</summary>
        <table>
            <tr>
                <td>Indicates the type of notification or update which you are sending<br>
                Default: 03 (Notification confirmed on publication)</td>
            </tr>
            <tr>
                <td>Required</td>
            </tr>
        </table>
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
    <details>
        <summary>DescriptiveDetail</summary>
        <details>
            <summary>ProductComposition</summary>
        </details>
        <details>
            <summary>ProductForm</summary>
        </details>
        <details>
            <summary>ProductFormDetail</summary>
        </details>
        <details>
            <summary>PrimaryContentType</summary>
        </details>
        <details>
            <summary>Measure</summary>
            <details>
                <summary>MeasureType</summary>
            </details>
            <details>
                <summary>Measurement</summary>
            </details>
            <details>
                <summary>MeasureUnitCode</summary>
            </details>
        </details>
        <details>
            <summary>EpubLicense</summary>
            <details>
                <summary>EpubLicenseName</summary>
            </details>
            <details>
                <summary>EpubLicenseExpression</summary>
                <details>
                    <summary>EpubLicenseExpressionType</summary>
                </details>
                <details>
                    <summary>EpubLicenseExpressionLink</summary>
                </details>
            </details>  
        </details>
        <details>
            <summary>TitleDetail</summary>
            <details>
                <summary>TitleType</summary>
            </details>
            <details>
                <summary>TitleElement</summary>
                <details>
                    <summary>TitleElementLevel</summary>
                </details>
                <details>
                    <summary>TitleText</summary>
                </details>
                <details>
                    <summary>Subtitle</summary>
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