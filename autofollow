const Nightmare = require('nightmare');
const nightmare = Nightmare({
    show: true,
    webPreferences: {
        partition: 'nopersist',
    },
});

const username = 'davi_gans132';
const password = 'aoyama';
const username = 'bapet7';
const password = 'aoyama';
const username = 'bleksiblek4';
const password = 'aoyama';
const username = 'yahyaku02';
const password = 'aoyama';
const username = 'counakracing';
const password = 'aoyama';
const search = '#kartinismanta';
const comment = 'keren';
const posts = 1;

nightmare
    .goto('http://instagram.com')
    .wait('._b93kq')
    .click('._b93kq') // log in option
    .wait('input[name=username]')
    .insert('input[name=username]', username)
    .insert('input[name=password]', password)
    .click('button') // btn login
    .wait('input[placeholder=Search]')
    .insert('input[placeholder=Search]', search)
    .wait('._gimca')
    .click('._gimca') // top suggest
    .wait('._mck9w')
    .click('._mck9w a') // click post
    .wait('._eszkz');

for (let i = 0; i < posts; i++) {
    nightmare.wait(1000)
        .click('._eszkz') // like
        .insert('._bilrf', comment) // comment
        .type('._bilrf', '\u000d')
        .click('._3a693'); // next
}

nightmare
    .wait(1000)
    .end()
    .then(function () {
        console.log('success');
    })
    .catch(function (err) {
        console.log(err);
    });
