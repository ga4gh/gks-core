# gkm-core

Core classes and schemas used by all GKM specifications (ie. VR, Cat-VRS, VA, etc..)

For more info
[GKM Repository Organization](https://docs.google.com/document/d/16SrjqPJ1ct_z8OK6kNcu3KO1ia6LAyVriSbuDLXRAI8/edit)

## Installing for development

Fork the repo at <https://github.com/ga4gh/gkm-core>.

    git clone git@github.com:YOUR_GITHUB_ID/gkm-core.git
    cd gkm-core
    make devready
    source venv/3.12/bin/activate
    pre-commit install

## Contributing to the schema

GKM Core uses the following source document for JSON Schema:

* [gkm-core-source.yaml](./schema/gkm-core/gkm-core-source.yaml)

To create the corresponding def and json files after making changes to any of of the
source documents, from the root directory:

    cd schema
    make all

> _Note: We have a custom pre-commit hook to run these commands after you stage a source
> document_

## Testing

To run the tests:

    (from the root directory of the project)
    make test
