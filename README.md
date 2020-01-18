# ph-ids
Philippines identification cards and their number formats. 

(Work in progress...)


    const PH_ID_LIST = [
        {
            key: 'UMID',
            name: 'Unified Multi-Purpose ID',
            prefix: 'CRN',
            format: /^\d{4}-\d{7}-\d{1}$/, // Match: 0123-1234567-1, 012-1234567-1, 01-1234567-1, 1-1234567-1,   Non-match: 123456789
        },
        {
            key: 'DL',
            name: 'Drivers License',
            prefix: '',
            format: /^([a-zA-Z0-9]){3}-\d{2}-\d{6}$/, // Match: F05-12-123456
        },
        {
            key: "PP",
            name: "Passport",
            prefix: '',
            format: /^([a-zA-Z0-9]){9}$/, // Match: P1234560A
        },
        {
            key: "POSTAL",
            name: "Postal ID",
            prefix: 'PRN',
            format: /^([a-zA-Z0-9]){12} ([a-zA-Z]){1}$/, // Match: A123456789012 P
        }
    ]